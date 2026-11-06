# rb-sdk C++ SDK 0.11.4 (stable)

이 브랜치는 `0.11.4` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.4
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.4

## sha256
```
bad224df3ab276cfb5460aa451842bbb51dd23171927d30988fcfe6e918a0c48  ./rainbow-rb-sdk_0.11.4_amd64.deb
f6274e0aa624f91085e0d66c2e3fc0047c02655fb066379acac86bc4abdc8100  ./rainbow-rb-sdk_0.11.4_arm64.deb
9609b970a401b1762caff7815e2c52e27e36b88640a29ee2b2e0ffdfc7c3390f  ./rainbow-rb-sdk-dev_0.11.4_amd64.deb
2c8a4ffdbecd38aaef894339d5cebc8af4d12bec4d0c96a8d0abc9e578b73993  ./rainbow-rb-sdk-dev_0.11.4_arm64.deb
e7403a855bf56c1c181f39315407054e2422ab31d6dbc8f42add2864879ee325  ./rb-sdk-cpp-0.11.4-aarch64-unknown-linux-gnu.tar.gz
65f24d91dad0e16320766248e912e50ca7ac951543b2d24a215fb7357c11d8aa  ./rb-sdk-cpp-0.11.4-x86_64-unknown-linux-gnu.tar.gz
574ce6f343eb32e8b236bac87fd96167bd5fb6a369a4c2ecbdc7595ca75a9d32  ./rb-sdk-cpp-0.11.4-x86_64-pc-windows-gnu.zip
```
