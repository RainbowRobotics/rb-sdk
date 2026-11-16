# rb-sdk C++ SDK 0.11.8 (stable)

이 브랜치는 `0.11.8` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.8 rainbow-rb-sdk=0.11.8 rainbow-rb-zenoh-dev=0.11.8 rainbow-rb-zenoh=0.11.8
sudo apt install rainbow-rb-zenoh-dev=0.11.8 rainbow-rb-zenoh=0.11.8   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.8

## sha256
```
359902a57622e32935e18d8ba333339277acaf6a53edc3c9400bde9ccdc4f0ec  ./rainbow-rb-sdk_0.11.8_amd64.deb
de6dd5fad1937a1e11668f6ddaac5a7c3a6a1b0459602b60dd4e40875b8e1035  ./rainbow-rb-sdk_0.11.8_arm64.deb
c0bfff2ab816a082b241a321a0537c143b96c9535c0df25f740e91962c8618bf  ./rainbow-rb-sdk-dev_0.11.8_amd64.deb
8635581e6372d51a658db47b7ed9c064c6ea0bce68e32d3783cf0d67fe074ef7  ./rainbow-rb-sdk-dev_0.11.8_arm64.deb
c245381e60809765c54cec3c3b51654adf0d02babb1acb3488e9ec4c402c12e9  ./rainbow-rb-zenoh_0.11.8_amd64.deb
7f9b6b847051171b0694174fc3ce8b1456eed18f6506b527d635be76bca4c2ce  ./rainbow-rb-zenoh_0.11.8_arm64.deb
ba3e0f1fa2d9c4f2b6b68c47feb8dd00ee7649b1f6adedc540d4c4197b2f5c97  ./rainbow-rb-zenoh-dev_0.11.8_amd64.deb
f3ff37acef162b5d68c0f68b5d91b1cbe03486586fba6ee5ddcdf64ac21a6015  ./rainbow-rb-zenoh-dev_0.11.8_arm64.deb
b560ca8fbff20d022853777dd5b36cf6ba7fa4b427dc146dcb8e5cb60dff82b9  ./rb-sdk-cpp-0.11.8-aarch64-unknown-linux-gnu.tar.gz
32c1cdd107bf6cb32e5c9e8b47c3233962f863ce250a9cef4a543101c0934eb9  ./rb-sdk-cpp-0.11.8-x86_64-unknown-linux-gnu.tar.gz
e151ec27e4a24e96384b7a6eff0091f32af7331310ac36634076611f916cfd3c  ./rb-sdk-cpp-0.11.8-x86_64-pc-windows-gnu.zip
```
