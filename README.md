# rb-sdk C++ SDK 0.1.2 (stable)

이 브랜치는 `0.1.2` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.2
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.2

## sha256
```
213e8cc15aae79aa2e7ce1595571a45665bcc29262b7ad4431ff0c8629d19371  ./rainbow-rb-sdk_0.1.2_amd64.deb
ba838bf97e44ecf1756e6f71653b39c6c288e51f1687c37e4c00548f43039a8c  ./rainbow-rb-sdk_0.1.2_arm64.deb
bbb45c07b294899f53d47716bc8bee6801bc3b92dd80b66ab8dc93b9cca4e516  ./rainbow-rb-sdk-dev_0.1.2_amd64.deb
05aa4a09021c3b736564b714ecafdf56452576d3ebb80d49b628f254c50071a2  ./rainbow-rb-sdk-dev_0.1.2_arm64.deb
725a4f918835fbe72ff51e0a47a793af26ce73f8b59fda14885946a705100baf  ./rb-sdk-cpp-0.1.2-aarch64-unknown-linux-gnu.tar.gz
4c2f199973af46cb962400d97aa466f2e8fa8a27cb95bdd64259d721715048c7  ./rb-sdk-cpp-0.1.2-x86_64-unknown-linux-gnu.tar.gz
511cfdc532f3b8988903ce45086d77f3a8458c1049098e1f2b029b4bebdd8def  ./rb-sdk-cpp-0.1.2-x86_64-pc-windows-gnu.zip
```
