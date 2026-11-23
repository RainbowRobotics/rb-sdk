# rb-sdk C++ SDK 0.11.14 (stable)

이 브랜치는 `0.11.14` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.14 rainbow-rb-sdk=0.11.14 rainbow-rb-zenoh-dev=0.11.14 rainbow-rb-zenoh=0.11.14
sudo apt install rainbow-rb-zenoh-dev=0.11.14 rainbow-rb-zenoh=0.11.14   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.14

## sha256
```
8fb1ae16338fec8e92c1827a9bb48f716abe33a5484426d1f241e8bf697ec550  ./rainbow-rb-sdk_0.11.14_amd64.deb
71a471aa8d1d005ef35a98a85328a851882d0a70783cb01a0a707b6b58ddc19b  ./rainbow-rb-sdk_0.11.14_arm64.deb
a11edac29d8dbd040c03b05f812482cec5ff8ff8b8d71a4efc3ae5907b8cad18  ./rainbow-rb-sdk-dev_0.11.14_amd64.deb
4aa96fa6e5e70874fa91d692bdb8c89f3701c8027649e2d6c719682eb7765fb1  ./rainbow-rb-sdk-dev_0.11.14_arm64.deb
c09e5a999a6243cefbaa58c661d9b6ec10af6fce31fe5f6c7282fd3c233c704a  ./rainbow-rb-zenoh_0.11.14_amd64.deb
45978a391a5a9c5f7a34b2b133e75289a522bc3cb788e8a5a91a3656b962223d  ./rainbow-rb-zenoh_0.11.14_arm64.deb
3bc360155c57890f3bb7bc4202552478bc197cbf0fc3baecaa2e7705d162e3f9  ./rainbow-rb-zenoh-dev_0.11.14_amd64.deb
9d94855c51dc5a3b7efc67e8c0656d1fae6f6ed617732a0e7a0aee9206b44c04  ./rainbow-rb-zenoh-dev_0.11.14_arm64.deb
028645759b60e115e0f2400fc97422ef20260b6d89bca6a9c67f509aeef85947  ./rb-sdk-cpp-0.11.14-aarch64-unknown-linux-gnu.tar.gz
62b87e1fb3eb5d240d954915e281f75cc8d2e179bdcbe7001d91bef65c6e8481  ./rb-sdk-cpp-0.11.14-x86_64-unknown-linux-gnu.tar.gz
6302e657f580ef4281cac621e1418f98d8770716919fc7adba92301887840c3f  ./rb-sdk-cpp-0.11.14-x86_64-pc-windows-gnu.zip
```
