# rb-sdk C++ SDK 0.1.2.dev4 (dev)

이 브랜치는 `0.1.2.dev4` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.2~dev4
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.2.dev4

## sha256
```
cdb138b72e58a24b3a46aa73a8377943de8d4f9aac76a8d23a69f1100ad84bd1  ./rainbow-rb-sdk_0.1.2~dev4_amd64.deb
f414ce37856f4adcef934d203e3c68647d392c7c64ee91c1d05dbc9110b3379f  ./rainbow-rb-sdk_0.1.2~dev4_arm64.deb
863a958b05cde764e655a70971522953566109ce2317f57cccc9a9a0e64f8fca  ./rainbow-rb-sdk-dev_0.1.2~dev4_amd64.deb
591f36234b045eee7a47d88e18237e76fc8614b873ff1e1fec177b0a609434e7  ./rainbow-rb-sdk-dev_0.1.2~dev4_arm64.deb
dc22746e7a3760221b8a45b3633dc465a89894addffd91a878eb270ceb79b987  ./rb-sdk-cpp-0.1.2.dev4-aarch64-unknown-linux-gnu.tar.gz
2d0366de0f414f679eaa132674da80fa4f112c2f637b0bd611a987ab62e5a129  ./rb-sdk-cpp-0.1.2.dev4-x86_64-unknown-linux-gnu.tar.gz
2435ef40cadb55507f96a5c721a6ef4b7e4e1684ac1b505bb73b9183d1c55b04  ./rb-sdk-cpp-0.1.2.dev4-x86_64-pc-windows-gnu.zip
```
