# rb-sdk C++ SDK 0.1.2.dev2 (dev)

이 브랜치는 `0.1.2.dev2` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.2~dev2
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.2.dev2

## sha256
```
b3fbf19fd7d331b261a455b5fdd40bc10997b6c3a30ea85d9c380f0309bdd0eb  ./rainbow-rb-sdk-dev_0.1.2~dev2_amd64.deb
544d475f7495a9be0d404a4eeaf216209b808055d00304ba44298949f630199d  ./rainbow-rb-sdk-dev_0.1.2~dev2_arm64.deb
03b99e1c0676877b74d5e8ebefeb37ec3b6b656f9755d29d2568cffa425800a6  ./rainbow-rb-sdk_0.1.2~dev2_amd64.deb
8e8814af2f5eafd8197879c1d43c2b6490109c4794d94f5078692e3c239ff303  ./rainbow-rb-sdk_0.1.2~dev2_arm64.deb
ed32987b75a9f578ac36d79d9a98a6586999ab91cf4f8886a00e25b453439a68  ./rb-sdk-cpp-0.1.2.dev2-aarch64-unknown-linux-gnu.tar.gz
1d6baeaf4d6af0e4b454004a36f0886a3eca100e29f3cffd493924ac6eaa19f5  ./rb-sdk-cpp-0.1.2.dev2-x86_64-unknown-linux-gnu.tar.gz
```
