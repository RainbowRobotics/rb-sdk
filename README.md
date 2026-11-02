# rb-sdk C++ SDK 0.11.2 (stable)

이 브랜치는 `0.11.2` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.2
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.2

## sha256
```
cd3ad5cd48d99c4fefceab717339022277ce48b97aac748b6a21678cec9c250e  ./rainbow-rb-sdk_0.11.2_amd64.deb
8ad6e347504c7af7396f702f05c18c7555bac74c7276fb4a921d90232e9386e9  ./rainbow-rb-sdk_0.11.2_arm64.deb
ac6cd2bb7078586798d1098f02bebfc31e22c4e49a69a5b37415cb76dd9a88e7  ./rainbow-rb-sdk-dev_0.11.2_amd64.deb
666f5c0303ea25dcdb7cafbe4712acf2fcdc798c070f49b23bd95a0b149dc96f  ./rainbow-rb-sdk-dev_0.11.2_arm64.deb
ea3d9d659a7dc4fefa3bef7103ed8827d9e0680160d3149aef5c5b8f5b350be1  ./rb-sdk-cpp-0.11.2-aarch64-unknown-linux-gnu.tar.gz
74f349463dee72211670d97c771d04628b4b6b19692b6cb674092141640d5686  ./rb-sdk-cpp-0.11.2-x86_64-unknown-linux-gnu.tar.gz
7dcf3dfc539a567684bca912080c845e4d834eba699e944d428e6d1298a7a9a8  ./rb-sdk-cpp-0.11.2-x86_64-pc-windows-gnu.zip
```
