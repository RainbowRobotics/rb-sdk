# rb-sdk C++ SDK 0.1.3 (stable)

이 브랜치는 `0.1.3` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.3
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.3

## sha256
```
74a2f776a3f7ef0c881447765729f2239e2409a95c1c342139d5dacc75967036  ./rainbow-rb-sdk_0.1.3_amd64.deb
4f2a7829a5c0380186caf6d42d3eddb5269dc822b0c8551cb4b4e3a05baae166  ./rainbow-rb-sdk_0.1.3_arm64.deb
4d4da541fac13e7efdd022ddeebb44455a3a3c622fb2522baa2f3106fa60bd6e  ./rainbow-rb-sdk-dev_0.1.3_amd64.deb
8b2952dfee42543f9658b245b75d03fab1556e77096ed89bf341fb9ae0957c32  ./rainbow-rb-sdk-dev_0.1.3_arm64.deb
6e06b3b27beebfb6b4b52a9496b211b9160f4c5d11e3fb71e792d1fe6506ad73  ./rb-sdk-cpp-0.1.3-aarch64-unknown-linux-gnu.tar.gz
43428e8750561ed52008068c1bd15dd5565a51944b6d8cd2ee622c2256a0cc95  ./rb-sdk-cpp-0.1.3-x86_64-unknown-linux-gnu.tar.gz
4afb0df3fc8501d1554f663d5c4dc486ccd7ad77ac8548523c4653bd8867c76c  ./rb-sdk-cpp-0.1.3-x86_64-pc-windows-gnu.zip
```
