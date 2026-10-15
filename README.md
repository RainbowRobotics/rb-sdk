# rb-sdk C++ SDK 0.10.2 (stable)

이 브랜치는 `0.10.2` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.2
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.2

## sha256
```
dbae52f5f07cc5376c24f76a477d1b83e70a5e15cde07ac53f2a41d3640becd9  ./rainbow-rb-sdk_0.10.2_amd64.deb
00a864ed7895f8e73b59b92768ae25334481472cc1204e9314574ea6e91ef40b  ./rainbow-rb-sdk_0.10.2_arm64.deb
74836e1599e32477bd944d744af9bf61b19db613117fa110aadcdbef23f4e4db  ./rainbow-rb-sdk-dev_0.10.2_amd64.deb
f6c09ccf0f733b11132274bf07f0025436dfed80556291426ea02bf814ce5396  ./rainbow-rb-sdk-dev_0.10.2_arm64.deb
65f7494a4545173d8544cb7181da22f26ac31047785ed61339e4aa43f9f2f409  ./rb-sdk-cpp-0.10.2-aarch64-unknown-linux-gnu.tar.gz
fff61b5129090e2f9d3142ba678152ae6a0cc4d114bf63af9f6fa01eb6f0f956  ./rb-sdk-cpp-0.10.2-x86_64-unknown-linux-gnu.tar.gz
3ecc57f71de786404543e536a885c5a6bbdd78d9f1f96c927ea7c08e4200bfd7  ./rb-sdk-cpp-0.10.2-x86_64-pc-windows-gnu.zip
```
