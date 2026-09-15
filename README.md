# rainbow-rb-sdk

APT repository + release archives for the Rainbow Robotics C++ SDK (`librb_sdk`).
The `main` branch itself carries no source code — just the workflow that publishes/manages
the package repository, plus the repository's signing public key.

## Install (Ubuntu / Debian, APT)

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key \
  | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main" \
  | sudo tee /etc/apt/sources.list.d/rb-sdk.list
# arm64 host: arch=arm64. Need a prerelease build? use "dev" instead of "stable".

sudo apt update
sudo apt install rainbow-rb-sdk-dev
```

Pin an exact version:

```bash
apt-cache madison rainbow-rb-sdk-dev
sudo apt install rainbow-rb-sdk-dev=1.2.3 rainbow-rb-sdk=1.2.3
# dev channel: rainbow-rb-sdk-dev=1.2.3~dev4 rainbow-rb-sdk=1.2.3~dev4
```

## Download (GitHub Releases)

If you just need the binaries without APT (CI, Docker builds, …), grab the platform tarball from
[Releases](https://github.com/RainbowRobotics/rb-sdk/releases) instead. APT traffic counts against
the GitHub Pages bandwidth limit, so CI should prefer this route over APT.

```bash
V=1.2.3
TRIPLE=x86_64-unknown-linux-gnu   # arm64: aarch64-unknown-linux-gnu
curl -fL "https://github.com/RainbowRobotics/rb-sdk/releases/download/$V/rb-sdk-cpp-$V-$TRIPLE.tar.gz" \
  | sudo tar -xzf - -C /usr/local
# CMake: find_package(rb_sdk PATHS /usr/local/lib/cmake/rb_sdk REQUIRED)
# pkg-config: PKG_CONFIG_PATH=/usr/local/lib/pkgconfig pkg-config --cflags --libs rb_sdk
```

> Do not load `librb_sdk.so.<version>` and the Python package `rainbow.rb_sdk` in the same process.

## Repository layout (by branch)

| Branch | Role |
|---|---|
| `main` | You are here. Holds the `publish-apt-repo` workflow and the repo's signing public key (`rb-sdk-apt-repo.gpg.key`) |
| `gh-pages` | The actual APT repository served via GitHub Pages (`dists/`, `pool/`). An orphan branch rewritten wholesale on every publish |
| `release/cpp/<version>` | Orphan branch holding just one version's artifacts (4 `.deb`s + 2 tarballs + sha256). The GitHub Release tag is retargeted to point here |

APT repository site: https://rainbowrobotics.github.io/rb-sdk/

Signing key fingerprint: `605E 8364 5698 465E 1452 CBF0 C749 1A44 F2FB 92C6`
