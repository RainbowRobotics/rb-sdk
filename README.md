# rb-sdk C++ SDK 0.11.9 (stable)

이 브랜치는 `0.11.9` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.9 rainbow-rb-sdk=0.11.9 rainbow-rb-zenoh-dev=0.11.9 rainbow-rb-zenoh=0.11.9
sudo apt install rainbow-rb-zenoh-dev=0.11.9 rainbow-rb-zenoh=0.11.9   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.9

## sha256
```
d675dead7383f378bc09ed27e869c9349c086e8d1c2919cc56138144927e87e2  ./rainbow-rb-sdk_0.11.9_amd64.deb
5ef82e2f2010de9354f65fc9d8e165329abe57c8dd4703ba41dd37b93971691b  ./rainbow-rb-sdk_0.11.9_arm64.deb
8c9f468cd38994e0e64f3c24d004847d37fd98884d42ed45404fcc23e0cf01cd  ./rainbow-rb-sdk-dev_0.11.9_amd64.deb
45542787fb08ed2bf6b8a7331a972d0a225b98961d33f2a4d0e7e4a144a36129  ./rainbow-rb-sdk-dev_0.11.9_arm64.deb
d7a98233cd8e22bccf0c437e420b766972d67ccb41fad02f5ebc6ceb44768ba2  ./rainbow-rb-zenoh_0.11.9_amd64.deb
22f93ad1a0d9216c17075517cd70cb1662b980f07075d37b5a6baff59b0c3009  ./rainbow-rb-zenoh_0.11.9_arm64.deb
6f89ba9733cd1392a763675a9e7bf8166906e0086a2a2e060e0ae695311ebed9  ./rainbow-rb-zenoh-dev_0.11.9_amd64.deb
43fd2cbba62f6be4bb718142edf35c799a58f236d62b69b0564e371ca11d3566  ./rainbow-rb-zenoh-dev_0.11.9_arm64.deb
34b416762c738a0c745884a572a00b497ec48deaa4e7f3da4fe1e9ee19239de2  ./rb-sdk-cpp-0.11.9-aarch64-unknown-linux-gnu.tar.gz
9568b5c793d31ad266c058b187b894d8444c1a9c96faff368ea8f6792b93a530  ./rb-sdk-cpp-0.11.9-x86_64-unknown-linux-gnu.tar.gz
79a691accfc482ad46e400213d707595c2c6ee28c659f99ef641c404a3af03f1  ./rb-sdk-cpp-0.11.9-x86_64-pc-windows-gnu.zip
```
