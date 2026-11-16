# rb-sdk C++ SDK 0.11.8.dev1 (dev)

이 브랜치는 `0.11.8.dev1` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk dev main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.8~dev1 rainbow-rb-sdk=0.11.8~dev1 rainbow-rb-zenoh-dev=0.11.8~dev1 rainbow-rb-zenoh=0.11.8~dev1
sudo apt install rainbow-rb-zenoh-dev=0.11.8~dev1 rainbow-rb-zenoh=0.11.8~dev1   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.8.dev1

## sha256
```
8e4ef2f24f8ed0c0ebe0bd3cb23dbedfb3026f7de6fddae12af31dfd2a4c02c8  ./rainbow-rb-sdk_0.11.8~dev1_amd64.deb
d29caef3bf06f0f21f827b00bc267fe8d54ba025f76947f2fc76d4ea6625394f  ./rainbow-rb-sdk_0.11.8~dev1_arm64.deb
18290ed7da8e26de0e3f0b300c0e5c31d303fb5fedaeb7afdc8d3ec3123b3496  ./rainbow-rb-sdk-dev_0.11.8~dev1_amd64.deb
28bcf4815026de354713be8f075d71ad14ce8edf18eba545b6f2ed6ad8e339b8  ./rainbow-rb-sdk-dev_0.11.8~dev1_arm64.deb
d00ab0d5a415f44c185f8a06787d46db6ac4c28025adf8537f44031d4517dfcb  ./rainbow-rb-zenoh_0.11.8~dev1_amd64.deb
0131ce6eba57de48cb8acf08744d20974d2a196fb1da85d62929fee9c3af00dd  ./rainbow-rb-zenoh_0.11.8~dev1_arm64.deb
3a584ad4e2310092e5bb8b5cec92f778a35c34ff6edeaaf8d3857f66e1b76b7c  ./rainbow-rb-zenoh-dev_0.11.8~dev1_amd64.deb
38927a77a9681c77516c8a27b689e8b88eaaa58b1a27d313a38584c28ecd4ae7  ./rainbow-rb-zenoh-dev_0.11.8~dev1_arm64.deb
5dffd3b84e092b3f3b510f9a7e8f4296c29abc033d1fa6cc7bebcd49cc7bb431  ./rb-sdk-cpp-0.11.8.dev1-aarch64-unknown-linux-gnu.tar.gz
7beaffe651365e56945572b458b68811524c7de5da8de4bea62fc80b021869de  ./rb-sdk-cpp-0.11.8.dev1-x86_64-unknown-linux-gnu.tar.gz
fc7019c1fe55ecfb3ae6e9e07e4e055be5bf4bcf12e6541219d3c371cce82317  ./rb-sdk-cpp-0.11.8.dev1-x86_64-pc-windows-gnu.zip
```
