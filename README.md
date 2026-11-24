# rb-sdk C++ SDK 0.11.15 (stable)

이 브랜치는 `0.11.15` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.15 rainbow-rb-sdk=0.11.15 rainbow-rb-zenoh-dev=0.11.15 rainbow-rb-zenoh=0.11.15
sudo apt install rainbow-rb-zenoh-dev=0.11.15 rainbow-rb-zenoh=0.11.15   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.15

## sha256
```
73076e64ec32f84a61812a4316c119183fd92966ac715d336a6f59a7274ec18b  ./rainbow-rb-sdk_0.11.15_amd64.deb
5b1076ecce11432fa527b3e8332cc9c37011c38c1a9e201320c4430bfa043442  ./rainbow-rb-sdk_0.11.15_arm64.deb
3e44891d11acf0ca41b048c94af2e0f023b0a4e689e63f5b3ec910972a9e2489  ./rainbow-rb-sdk-dev_0.11.15_amd64.deb
8c75a5e19728e7f87323ff8b5dfa329b27f15ff446659a3703db284bea1a5c03  ./rainbow-rb-sdk-dev_0.11.15_arm64.deb
14cb81955524e444f75dc27bc1e86c455ae32f6406c7309af7b32e6cb30772b3  ./rainbow-rb-zenoh_0.11.15_amd64.deb
46f151468b2e2a76ada09be598b22e9bfb7fa87a53916fb28d7179eda7cfdf8f  ./rainbow-rb-zenoh_0.11.15_arm64.deb
6ce80a51d4cd298a65d1de9f28630601ccfb79835f2a210c15faee7924cee0b3  ./rainbow-rb-zenoh-dev_0.11.15_amd64.deb
668b6f2e183e5854dcd717ddd59b6b6611f5b0a15542a4661360b31f690de351  ./rainbow-rb-zenoh-dev_0.11.15_arm64.deb
b8662b432f0b416c70d721ed7bf191f16d095a7d5fa5a1d11c598d0b4d29f1b2  ./rb-sdk-cpp-0.11.15-aarch64-unknown-linux-gnu.tar.gz
5adc7bacbaa38473c374cea9797013e1b7bc63a209e296902425d211d6c3445e  ./rb-sdk-cpp-0.11.15-x86_64-unknown-linux-gnu.tar.gz
11909970afd5a72ee23010144723a97b9e667b4577b2646eca18385bf9d18766  ./rb-sdk-cpp-0.11.15-x86_64-pc-windows-gnu.zip
```
