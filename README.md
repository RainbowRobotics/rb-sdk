# rb-sdk C++ SDK 0.11.7 (stable)

이 브랜치는 `0.11.7` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.7
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.7

## sha256
```
7b5c89b758b93ee018acd8bdde33f297b14279f88858fa7988344557b2039c8e  ./rainbow-rb-sdk_0.11.7_amd64.deb
2ee477c3c806c7cfa22ae26e91550c646f0152d1eaf271f9c119771cc3b4dc5b  ./rainbow-rb-sdk_0.11.7_arm64.deb
83a960f2859708e550532ca16d72771bce44d0b5be7f75ee8b66b1a96cea9bb9  ./rainbow-rb-sdk-dev_0.11.7_amd64.deb
0dc27856466b5ad10813221bbbd2e29d11e4ad000fef3273fab088fcbb145e28  ./rainbow-rb-sdk-dev_0.11.7_arm64.deb
c36c6f1652439226651e72d4ffff24d71c7adb7c3ecb7310ea46001dd07b0097  ./rb-sdk-cpp-0.11.7-aarch64-unknown-linux-gnu.tar.gz
a3ae81b806961f1e089438aa8a4c84e6f2ee32e12411c8478f36e0373a1cca94  ./rb-sdk-cpp-0.11.7-x86_64-unknown-linux-gnu.tar.gz
52d7d39136e9659fa92ac84b5dc8e140bc1271d69faaca09f023a98e3fd1c2d0  ./rb-sdk-cpp-0.11.7-x86_64-pc-windows-gnu.zip
```
