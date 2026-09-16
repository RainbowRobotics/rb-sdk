# rb-sdk C++ SDK 0.1.2.dev3 (dev)

이 브랜치는 `0.1.2.dev3` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.2~dev3
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.2.dev3

## sha256
```
cdb0407c7366ae6ad1bac98ee761852937198883065287c1a96df56f94e784a7  ./rainbow-rb-sdk_0.1.2~dev3_amd64.deb
d343d7cf7a4b014fba158322c68d108a182168cbdb1f4a7c1601c14e788af4e3  ./rainbow-rb-sdk_0.1.2~dev3_arm64.deb
f7e947e30c5388f54c32a860b83cd75ef3b917731b10cf6d9d357b80cfb2c8d0  ./rainbow-rb-sdk-dev_0.1.2~dev3_amd64.deb
ef9bdb96792a63d167e8b0c6a5b0eb52a8ff6c27183c2221258c1ac30b37b56a  ./rainbow-rb-sdk-dev_0.1.2~dev3_arm64.deb
68c6f7a1f65ee4bd59807e565b8028cde6a1bc19808138ff4f65de2b3aca8362  ./rb-sdk-cpp-0.1.2.dev3-aarch64-unknown-linux-gnu.tar.gz
ccfcc3cd27b6a1e5ea864d80ee4068731b56c2b4c4296b8b4bb9e3fa1d5e1d45  ./rb-sdk-cpp-0.1.2.dev3-x86_64-unknown-linux-gnu.tar.gz
1062f65474fc9ec91a870da2a7f4e33a3b1611375a356b040748234a39bbcd0a  ./rb-sdk-cpp-0.1.2.dev3-x86_64-pc-windows-gnu.zip
```
