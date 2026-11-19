# rb-sdk C++ SDK 0.11.12 (stable)

이 브랜치는 `0.11.12` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.12 rainbow-rb-sdk=0.11.12 rainbow-rb-zenoh-dev=0.11.12 rainbow-rb-zenoh=0.11.12
sudo apt install rainbow-rb-zenoh-dev=0.11.12 rainbow-rb-zenoh=0.11.12   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.12

## sha256
```
8bd5c9fe65aeaddfd2a84996f724208a19b6e2f2c569e6de877f98313e4effde  ./rainbow-rb-sdk_0.11.12_amd64.deb
b2c585357f7df8b0a84c95766a68c70f3eb143a78f8dfb6b7056c2f1ca6a045c  ./rainbow-rb-sdk_0.11.12_arm64.deb
26be3eac09d94bccb8ba30f545c8e0f1108eb28be7350a34b51976907d8f2102  ./rainbow-rb-sdk-dev_0.11.12_amd64.deb
11ee04b0905a0b426994273fc4c8df67543b33e02907b9653ab01b78213e0979  ./rainbow-rb-sdk-dev_0.11.12_arm64.deb
14ab14c5a09b54fa6d3559ba09e75c14f7198057088840049622c9183be1b016  ./rainbow-rb-zenoh_0.11.12_amd64.deb
3aafbf01ca99a05ce7fa20ffad988b703e53193bedeea5142dfec223acd6f6f3  ./rainbow-rb-zenoh_0.11.12_arm64.deb
80f6dc34760e2e3c8413ebdf32776f927a227f0de7bce49154b5e6fd2a23835b  ./rainbow-rb-zenoh-dev_0.11.12_amd64.deb
ec4964193d3b06aee2c56ac352cfd65f792296d9560b539585b0c32ba3e88b05  ./rainbow-rb-zenoh-dev_0.11.12_arm64.deb
e714b1e95aba2df74da99cd20b98e2e2684ae58b8d79e9d2b40c2763da3155e8  ./rb-sdk-cpp-0.11.12-aarch64-unknown-linux-gnu.tar.gz
2834b852102febf7bc9ed65ed00a0da13e162c2ec0c14880b80082acb07d6d6b  ./rb-sdk-cpp-0.11.12-x86_64-unknown-linux-gnu.tar.gz
d4741881edc891bbdf545227bdae633e5f02cbd98226692ac2735079f17152c4  ./rb-sdk-cpp-0.11.12-x86_64-pc-windows-gnu.zip
```
