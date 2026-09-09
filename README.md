# rb-sdk C++ SDK 0.1.2.dev1 (dev)

이 브랜치는 `0.1.2.dev1` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.2~dev1
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.2.dev1

## sha256
```
65c1a14658cefdadc866772767b97929794bec90e9e5156618c7c4d6e095e1fa  ./rainbow-rb-sdk-dev_0.1.2~dev1_amd64.deb
a62c0079d362e1749a6c1061ff67ef441b1f6f6dd6bb4968931c51e8bc8a0699  ./rainbow-rb-sdk-dev_0.1.2~dev1_arm64.deb
767dbadbdfab8035acc65f5109e8ab8f8f83dfb2814e3cc8e3ebdc4171036d37  ./rainbow-rb-sdk_0.1.2~dev1_amd64.deb
d6a4cbef3a72980b14fbbb7ee057e4cd892df857dcbdfd752382b3385cc66ca4  ./rainbow-rb-sdk_0.1.2~dev1_arm64.deb
5c011e293671b140bedb2e660a0df4bb5b0798fc063bf9dcc469cd0a4ac45077  ./rb-sdk-cpp-0.1.2.dev1-aarch64-unknown-linux-gnu.tar.gz
4d40725530be97a20e159298840304c50228b1d1b0feeb0535aea32587bd06a1  ./rb-sdk-cpp-0.1.2.dev1-x86_64-unknown-linux-gnu.tar.gz
```
