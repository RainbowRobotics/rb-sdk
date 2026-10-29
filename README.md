# rb-sdk C++ SDK 0.10.4 (stable)

이 브랜치는 `0.10.4` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.4
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.4

## sha256
```
fb26c9eef742db7b296243e5c3268ebb93fb489ab45090271ebdcbbcb78c9736  ./rainbow-rb-sdk_0.10.4_amd64.deb
ac65858514a2edca9c9fac44ede8fa97065ba6bf26bd277cdb9d38a60a8f6006  ./rainbow-rb-sdk_0.10.4_arm64.deb
5aec711988fc0e23b8fd1c4918cfb30354431cae98cafa1ac8392f03688d07ce  ./rainbow-rb-sdk-dev_0.10.4_amd64.deb
0570758435aa79396add6424d8f0f2eabfd817da374f327da8f98d6d74b6bec9  ./rainbow-rb-sdk-dev_0.10.4_arm64.deb
c2b4a28b6fae0c2eff21030f55ba4eab44dd4bbfc90d980caf97bab624defec7  ./rb-sdk-cpp-0.10.4-aarch64-unknown-linux-gnu.tar.gz
ccd8eeb79b74889843a1098b7bfdd6252c108191be90a7e7fdf76311a9d05c3e  ./rb-sdk-cpp-0.10.4-x86_64-unknown-linux-gnu.tar.gz
5d6ec68492ea682216350796f669b577901a51b61f82cf0188c302ad59b0660d  ./rb-sdk-cpp-0.10.4-x86_64-pc-windows-gnu.zip
```
