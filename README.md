# Rainbow Robotics C++ SDK — APT repository

This branch (`gh-pages`) is served by GitHub Pages as the APT repository for the
Rainbow Robotics C++ SDK. It is an orphan branch with a rewritten single-commit
history — do not base source work on it.

```
https://rainbowrobotics.github.io/rb-sdk/
```

## Install (Ubuntu / Debian)

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key \
  | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main" \
  | sudo tee /etc/apt/sources.list.d/rb-sdk.list
# arm64 host: arch=arm64. dev channel: replace "stable" with "dev".

sudo apt update
sudo apt install rainbow-rb-sdk-dev
```

Pin an exact version while it is still in retention:

```bash
apt-cache madison rainbow-rb-sdk-dev
sudo apt install rainbow-rb-sdk-dev=1.2.3 rainbow-rb-sdk=1.2.3
# dev: sudo apt install rainbow-rb-sdk-dev=1.2.3~dev4 rainbow-rb-sdk=1.2.3~dev4
```

## CI / automated builds — use the release tarball, not APT

APT downloads count against the GitHub Pages bandwidth soft limit. CI should pull
the Linux binary tarball from the GitHub Release instead:

```bash
V=1.2.3
TRIPLE=x86_64-unknown-linux-gnu   # arm64: aarch64-unknown-linux-gnu
curl -fL "https://github.com/RainbowRobotics/rb-sdk/releases/download/$V/rb-sdk-cpp-$V-$TRIPLE.tar.gz" \
  | sudo tar -xzf - -C /usr/local
# CMake: find_package(rb_sdk PATHS /usr/local/lib/cmake/rb_sdk REQUIRED)
```

## Layout

```
.nojekyll
apt-ftparchive.conf                 Release field template (Origin/Label/…)
rb-sdk-apt-repo.gpg.key             repository signing public key (armored)
pool/{stable,dev}/*.deb             package pool, one directory per channel
dists/{stable,dev}/                 Release / InRelease / Release.gpg + Packages
```

Metadata is regenerated on every publish by `publish-apt-repo.yml` in the repo's
default branch. New versions can take a few minutes to appear after a push while
`pages-build-deployment` runs.

> Do not load `librb_sdk.so.<version>` and the Python package `rainbow.rb_sdk` in
> the same process.
