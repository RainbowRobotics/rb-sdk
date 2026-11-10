# rb-sdk C++ SDK 0.11.5 (stable)

이 브랜치는 `0.11.5` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.5
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.5

## sha256
```
747791a2b5e4c3eacb5f82b2c4ea23cff2c6f84cd0c1fbe77c725f4dfc015fe0  ./rainbow-rb-sdk_0.11.5_amd64.deb
44ea63a7305669c1571eee44d0c07c383bea1bcfc3fcf769b3d33ae87439f45f  ./rainbow-rb-sdk_0.11.5_arm64.deb
c2ce1fe2424eafdf7e3dbbee3dca9a56b164bd1f8d0ce5412f20659cb3b1e4b2  ./rainbow-rb-sdk-dev_0.11.5_amd64.deb
2103877be00b75ec841f12255576293ae52efe97bb00cb73ead2aa4e1f571693  ./rainbow-rb-sdk-dev_0.11.5_arm64.deb
5deeeae07d1719c6cb0085f2fa83e9acbaaa8f6f4312e161e8412f575ca4cfd4  ./rb-sdk-cpp-0.11.5-aarch64-unknown-linux-gnu.tar.gz
bfc4f8e11bd547223dcb43d3d28aa3f75dee57d5a47d1a34116ec00fc4b464c2  ./rb-sdk-cpp-0.11.5-x86_64-unknown-linux-gnu.tar.gz
c891899fc202b7f4a59028f45c77ee7ee8748e9df3303379e4b7532fee62d7fe  ./rb-sdk-cpp-0.11.5-x86_64-pc-windows-gnu.zip
```
