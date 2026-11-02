# rb-sdk C++ SDK 0.11.3 (stable)

이 브랜치는 `0.11.3` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.3
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.3

## sha256
```
92f8ec6060cb47c5332d8993e3c2d956548f9229499e6d36f73d55fa10ca0ccb  ./rainbow-rb-sdk_0.11.3_amd64.deb
0a791de87f2151233b9a538a3405a8f114fc54cd22c1325455433dce84c5f43e  ./rainbow-rb-sdk_0.11.3_arm64.deb
ffd9205083adb94a9740267582b9ba50e6ecb675f625fde092c8e93d0e4cf3d7  ./rainbow-rb-sdk-dev_0.11.3_amd64.deb
9fc2a7ae6c417cb082424da9e36254c897b56da550f22c566fefa55d2f586e27  ./rainbow-rb-sdk-dev_0.11.3_arm64.deb
293d566b272e6dbae3529d75ace26b59e59f7ed2378c7409b33aaadf1a352c9f  ./rb-sdk-cpp-0.11.3-aarch64-unknown-linux-gnu.tar.gz
2beb09e5ecdafbb7ebffd5c3ffc4c7fbfe37e4c46b1898f7aa166a4c60f9ff4e  ./rb-sdk-cpp-0.11.3-x86_64-unknown-linux-gnu.tar.gz
fbefb5ba28d8d5772f8e9ee8c82e6b770ab547ceb25fc837fbd09ce3de16f00b  ./rb-sdk-cpp-0.11.3-x86_64-pc-windows-gnu.zip
```
