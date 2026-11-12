<div align="center">

<img src="https://avatars.githubusercontent.com/u/151020060?s=200&v=4" width="96" alt="Rainbow Robotics" />

# Rainbow Robotics SDK

**One SDK for every Rainbow Robotics robot. Python and C++, same API.**

Drive cobots, AMRs and the RB-Y1 dual-arm robot through the Muscat runtime,
from the robot itself or from your laptop.

[![PyPI](https://img.shields.io/pypi/v/rainbow-rb-sdk?label=PyPI&color=3775A9&logo=pypi&logoColor=white)](https://pypi.org/project/rainbow-rb-sdk/)
[![Python](https://img.shields.io/badge/python-3.11%20%7C%203.12%20%7C%203.13-3776AB?logo=python&logoColor=white)](https://pypi.org/project/rainbow-rb-sdk/)
[![Release](https://img.shields.io/github/v/release/RainbowRobotics/rb-sdk?label=C%2B%2B%20SDK&color=E1251B&logo=cplusplus&logoColor=white)](https://github.com/RainbowRobotics/rb-sdk/releases/latest)
[![Docs](https://img.shields.io/badge/docs-latest-0A7BBB?logo=readthedocs&logoColor=white)](https://rainbowrobotics.github.io/rb-sdk/docs/latest/)
![Platforms](https://img.shields.io/badge/platform-Linux%20x86__64%20%7C%20Linux%20arm64%20%7C%20Windows-555)

### [📖 Documentation](https://rainbowrobotics.github.io/rb-sdk/docs/latest/) · [🐍 Python API](https://rainbowrobotics.github.io/rb-sdk/docs/latest/api/modules.html) · [⚙️ C++ API](https://rainbowrobotics.github.io/rb-sdk/docs/latest/api/cpp.html) · [📦 Downloads](https://rainbowrobotics.github.io/rb-sdk/)

</div>

---

## What you can control

| Robot | Python | C++ | What it covers |
|---|---|---|---|
| **Collaborative arm (cobot)** | `RBManipulateSDK` | `RBManipulateSDK` | move (J / L / blend), state stream, I/O, points, config, safety, flange, vision, programs |
| **AMR** | `RBAmrSDK` | `RBAmrSDK` | move, map, localization, sensors, status, lift and accessories |
| **RB-Y1 dual-arm** | `RBRby1SDK` | `RBRby1SDK` | power and servo, `move_j` / `move_l`, torso and arm gains, tool flange I/O. RB-Y1 C++ SDK is bundled, nothing extra to install |
| **Programs and plugins** | `RBProgramSDK` | `RBProgramSDK` | run, pause and stop programs, plugin calls, Modbus / RPC |

Everything goes over a [Zenoh](https://zenoh.io) mesh. On the robot it connects with no setup;
from another machine, one `connect()` call joins the mesh.

## Install

<table>
<tr><th>Python (3.11 – 3.13)</th><th>C++ (Ubuntu / Debian, APT)</th></tr>
<tr><td>

```bash
pip install rainbow-rb-sdk
```

macOS (editor autocompletion and type
checking only, no runtime):

```bash
pip install rainbow-rb-sdk-stubs
```

</td><td>

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key \
  | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] \
https://rainbowrobotics.github.io/rb-sdk stable main" \
  | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev
```

</td></tr>
</table>

Prerelease builds: use the `dev` channel in place of `stable` (APT) or `pip install --pre`.
Binary tarballs for Linux and a Windows (MinGW) zip are on the [download page](https://rainbowrobotics.github.io/rb-sdk/).

## Quick start

### Python: move the arm

```python
from rainbow.rb_sdk import RBManipulateSDK

arm = RBManipulateSDK()  # on the robot: joins the local mesh automatically

arm.move.call_move_j(
    robot_model="C500920",
    target={"tar_values": [0, 0, 0, 0, 0, 0], "tar_frame": 0, "tar_unit": 0},
)
```

### Python: connect from your laptop and stream state

```python
import time
from rainbow.rb_sdk import RBManipulateSDK
from rainbow.rb_sdk.rb_sdk_cpp import ConnectOptions
from rainbow.rb_flat_buffers.IPC.State_Core import State_CoreT

arm = RBManipulateSDK()

opts = ConnectOptions()
opts.host = "192.168.1.100"   # robot IP
opts.token = "<service token>"
arm.connect(opts)             # register subscriptions AFTER connect()

@arm.zenoh_subscribe("C500920/state_core", flatbuffer_obj_t=State_CoreT)
def on_state(*, obj_payload: State_CoreT | None, **_):
    if obj_payload:
        print("motion mode:", obj_payload.motionMode)

while True:
    time.sleep(1)
```

### C++: read the robot state

```cpp
#include "manipulate/rb_manipulate_sdk.hpp"
#include <cstdio>

int main() {
  RBManipulateSDK arm;

  ConnectOptions opts;
  opts.host  = "192.168.1.100";
  opts.token = "<service token>";
  arm.connect(opts);

  IPC::State_CoreT s = arm.state.state_core("C500920");
  for (float q : s.joint_q_ref) std::printf("%.3f ", q);
  std::printf("\n");
}
```

```cmake
find_package(rb_sdk REQUIRED)
target_link_libraries(my_app PRIVATE rb_sdk::rb_sdk)   # C++20 is propagated
```

More examples and every method's parameters, return types and timeouts are in the
**[documentation](https://rainbowrobotics.github.io/rb-sdk/docs/latest/)**.

## Packages

| Package | Where | Contents |
|---|---|---|
| `rainbow-rb-sdk` | PyPI | Python SDK (native wheels: Linux x86_64 / aarch64, Windows x64) |
| `rainbow-rb-sdk-stubs` | PyPI | Type stubs (PEP 561) for platforms without native wheels |
| `rainbow-rb-zenoh`, `rainbow-rb-flat-buffers`, `rainbow-rb-schemas`, … | PyPI | Transport, message types and schemas, installed as dependencies |
| `rainbow-rb-sdk` / `rainbow-rb-sdk-dev` | APT | `librb_sdk.so` runtime / headers + CMake and pkg-config files |
| `rb-sdk-cpp-<ver>-<triple>.tar.gz` | [Releases](https://github.com/RainbowRobotics/rb-sdk/releases) | Relocatable Linux binaries (x86_64, aarch64). Use this in CI instead of APT |
| `rb-sdk-cpp-<ver>-x86_64-pc-windows-gnu.zip` | [Releases](https://github.com/RainbowRobotics/rb-sdk/releases) | Windows DLL for llvm-mingw / MSYS2 UCRT (not MSVC) |

Python and C++ releases share one version number. `rainbow-rb-sdk-dev` requires the exact same
`rainbow-rb-sdk` runtime version.

> [!WARNING]
> Do not load `librb_sdk.so` and the Python package `rainbow.rb_sdk` in the same process.
> Each embeds its own networking runtime.

## Versions and channels

| Channel | Python | APT | Docs |
|---|---|---|---|
| **stable** | `pip install rainbow-rb-sdk` | `stable` | [docs/latest](https://rainbowrobotics.github.io/rb-sdk/docs/latest/) |
| **dev** (prerelease) | `pip install --pre rainbow-rb-sdk` | `dev` | [docs/dev](https://rainbowrobotics.github.io/rb-sdk/docs/dev/) |

Older versions stay available from PyPI, `apt-cache madison rainbow-rb-sdk-dev` and the docs version switcher.

## About this repository

This repository only hosts the distribution. SDK source is not published here.

| Branch | Contents |
|---|---|
| `main` | This README and the APT signing public key `rb-sdk-apt-repo.gpg.key` |
| `gh-pages` | The site at [rainbowrobotics.github.io/rb-sdk](https://rainbowrobotics.github.io/rb-sdk/): APT repo (`dists/`, `pool/`) and versioned docs (`docs/`) |
| `release/cpp/<version>` | Archived `.deb`s and tarballs of one release (the release tag points here) |

APT signing key fingerprint: `605E 8364 5698 465E 1452 CBF0 C749 1A44 F2FB 92C6`

---

<div align="center">

Made by [Rainbow Robotics](https://www.rainbow-robotics.com) · Proprietary license

</div>
