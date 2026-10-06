# rb-sdk C++ SDK 0.1.6 (stable)

이 브랜치는 `0.1.6` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.6
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.6

## sha256
```
4c29baca245ed6ceff02112f16f3894db734a5b529dab23f5c050188c4ad0df9  ./rainbow-rb-sdk_0.1.6_amd64.deb
0c320149fd819eb4a883dcf698ad8a8495a5eb5ebcb518b66cccaf97470b641e  ./rainbow-rb-sdk_0.1.6_arm64.deb
b28fdec11529a59a865e23bf1d7a227b792e756450d0b0b744e416360a5d2910  ./rainbow-rb-sdk-dev_0.1.6_amd64.deb
05970f8b0f21554345d5f5d2d9e7bd7c5f33ab47c99f93056ba04d710f4c86f8  ./rainbow-rb-sdk-dev_0.1.6_arm64.deb
e49c60f3383f36dd2c89ac4bfbac36fdd7bc0c253e0b27a3cc7cf2fbf324d928  ./rb-sdk-cpp-0.1.6-aarch64-unknown-linux-gnu.tar.gz
27a8febd595fd074db371a63f54cb6433b7d03752d19123e36cde746d08fab65  ./rb-sdk-cpp-0.1.6-x86_64-unknown-linux-gnu.tar.gz
1d2226e352a3b3fad44a93f2c375db97179a418a31a15bf59ccc62c2298d139b  ./rb-sdk-cpp-0.1.6-x86_64-pc-windows-gnu.zip
```
