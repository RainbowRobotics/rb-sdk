# rb-sdk C++ SDK 0.11.6 (stable)

이 브랜치는 `0.11.6` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.6
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.6

## sha256
```
a9f636285be2e0df77a9ac96d5b5d484edec07f81d6c8747982d2bc3dfc17172  ./rainbow-rb-sdk_0.11.6_amd64.deb
3035bb6f06107b0a88e29753cff443530b9425d734f06bb62125bb5eb521f652  ./rainbow-rb-sdk_0.11.6_arm64.deb
bb0744b772fdb28d356cbd8e4d28cd2ae909fcc5cbd63b5ff76ea2373f5ba143  ./rainbow-rb-sdk-dev_0.11.6_amd64.deb
0fcdb93a61f20fafdcddbdadce199a041a9f8120e70fde7bef528c766a390dd1  ./rainbow-rb-sdk-dev_0.11.6_arm64.deb
57eec762b115a271a5082d6214b0893906b2b3ba79e2d6d477f9e2a496250439  ./rb-sdk-cpp-0.11.6-aarch64-unknown-linux-gnu.tar.gz
8d02f568875bef35cb47185b3364ee0fedfebaa689d739cd3dad8c1d423bc021  ./rb-sdk-cpp-0.11.6-x86_64-unknown-linux-gnu.tar.gz
f0d87542853a4e088648908ca14358c8d13c6b33b707fec6c7787360cffbfa2b  ./rb-sdk-cpp-0.11.6-x86_64-pc-windows-gnu.zip
```
