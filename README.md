# rb-sdk C++ SDK 0.1.4.dev1 (dev)

이 브랜치는 `0.1.4.dev1` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.4~dev1
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.4.dev1

## sha256
```
331ba83925a42f43131844f4f17cc2c7079d83654eb13e74250f7c852391e788  ./rainbow-rb-sdk_0.1.4~dev1_amd64.deb
ff4573c0dd2a789940d61862ad84d612956177457855fa2da653b3cafc84f857  ./rainbow-rb-sdk_0.1.4~dev1_arm64.deb
224b7c245634a5bd25e67ab945041925fb9a30c237d5826519206f38bad714e7  ./rainbow-rb-sdk-dev_0.1.4~dev1_amd64.deb
d3c975d867078bb86f724d139739329c59a40c7c028f8ac83149ebbab05ffb7b  ./rainbow-rb-sdk-dev_0.1.4~dev1_arm64.deb
3767800fa4b584895b5b50ab0f05f45a0503f2193dfe168f78ccfe116aaecd27  ./rb-sdk-cpp-0.1.4.dev1-aarch64-unknown-linux-gnu.tar.gz
0dc5b42d65471c95ceb76d0a224a30148d4a6534495c31c948a267c67edb840b  ./rb-sdk-cpp-0.1.4.dev1-x86_64-unknown-linux-gnu.tar.gz
5efbe8d795b2e7ef23720df0b1ee7051eac1aea1226b026a649d5f3669081325  ./rb-sdk-cpp-0.1.4.dev1-x86_64-pc-windows-gnu.zip
```
