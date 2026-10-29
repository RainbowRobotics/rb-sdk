# rb-sdk C++ SDK 0.10.6 (stable)

이 브랜치는 `0.10.6` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.6
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.6

## sha256
```
13b46b9ebad2e5c58bc2d90d138e0e954008e399fc6032ea3a1c21a09efc3af6  ./rainbow-rb-sdk_0.10.6_amd64.deb
8b3acb24ba556102da291ef5ec1fa19d53fc6a65d093263769093bfd275a82cb  ./rainbow-rb-sdk_0.10.6_arm64.deb
a5481e3a3cbe6b5336e9e02dd943490c7a75ee49778c22519e0d24aab2904e12  ./rainbow-rb-sdk-dev_0.10.6_amd64.deb
7286996669f9a51defc53a2b5d3bc5d94f51461227215a4049a68584f2ce75d9  ./rainbow-rb-sdk-dev_0.10.6_arm64.deb
17092b396807a3d976f19bf7d829a60bf0e0a8d0a7abee2b49ad25dcae57b4c8  ./rb-sdk-cpp-0.10.6-aarch64-unknown-linux-gnu.tar.gz
51e07f536eec97a75ff26a4718c5db3e1232e1328ac5f812470badd5c36c3972  ./rb-sdk-cpp-0.10.6-x86_64-unknown-linux-gnu.tar.gz
da6bd80e2ca45b4744d03925dc8628afcdc9c975a2dddd726859e62ef68c3908  ./rb-sdk-cpp-0.10.6-x86_64-pc-windows-gnu.zip
```
