# rb-sdk C++ SDK 0.1.7 (stable)

이 브랜치는 `0.1.7` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.7
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.7

## sha256
```
53cb250b08a58c11da3bf7c02b74c56f03c26f56cd2a0c86576c637867a1a517  ./rainbow-rb-sdk_0.1.7_amd64.deb
6d990bafdce377cd49ce5f090de0c8b083d02e8af6ff06f337bec06d1e5006f6  ./rainbow-rb-sdk_0.1.7_arm64.deb
30757f44582e0eb03555e21cebecb74be60657c01f3f23c85a2da73406cb7cc8  ./rainbow-rb-sdk-dev_0.1.7_amd64.deb
41df1852d259fcd2d932deca85fa4e967f62e724cdafcc9008dd4a2abf264c83  ./rainbow-rb-sdk-dev_0.1.7_arm64.deb
0d269aafc651da8b8ecb49a43db97e660b0daeb2c756f2d9eb50fbf235277ca5  ./rb-sdk-cpp-0.1.7-aarch64-unknown-linux-gnu.tar.gz
51dd6ce25809b1b84ee3603e18e68d00d6137c246f1649b3050963450b6c6686  ./rb-sdk-cpp-0.1.7-x86_64-unknown-linux-gnu.tar.gz
08104ee872ef8113d48291be0d01502343c2f780d08433f5f94dcc7089264cea  ./rb-sdk-cpp-0.1.7-x86_64-pc-windows-gnu.zip
```
