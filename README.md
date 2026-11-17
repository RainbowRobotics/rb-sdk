# rb-sdk C++ SDK 0.11.10 (stable)

이 브랜치는 `0.11.10` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.10 rainbow-rb-sdk=0.11.10 rainbow-rb-zenoh-dev=0.11.10 rainbow-rb-zenoh=0.11.10
sudo apt install rainbow-rb-zenoh-dev=0.11.10 rainbow-rb-zenoh=0.11.10   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.10

## sha256
```
b11c420d1a505446e6405cee8349d89d4981a72f7c7978195bf7c426cfb1cc66  ./rainbow-rb-sdk_0.11.10_amd64.deb
65d1b739d32ca39642c88645618ae77bb719d5854f175f1c9d9855508639534c  ./rainbow-rb-sdk_0.11.10_arm64.deb
00ac6bf72933bad02ba42c4b64ad2463082496e6ba42e48fe523b6b78cf11c78  ./rainbow-rb-sdk-dev_0.11.10_amd64.deb
f229f52339f0397b3a413fc14ad1a9febc8d3769a11af66c6922b522ae61c051  ./rainbow-rb-sdk-dev_0.11.10_arm64.deb
5070958a9e6ca87c4506bb7117c1a59bfced1f0194788cac8ef881c8f9d4d157  ./rainbow-rb-zenoh_0.11.10_amd64.deb
da0e0bb1a8d976f83a02b2299a520af144273039a3ecf3677f7cb1f4d3649db6  ./rainbow-rb-zenoh_0.11.10_arm64.deb
c6036d3ef9818f078a8e5dcf79f814634e5464826b2b19240182a7c8a72eb3d9  ./rainbow-rb-zenoh-dev_0.11.10_amd64.deb
9076efefa0fa3175818e1d2e576b6ef8e58c2dc0ba1215716c76cea732a91f4f  ./rainbow-rb-zenoh-dev_0.11.10_arm64.deb
d4fe88e8aa8e3c3726d0f992fe220e383a1dfd7742c2af95e7c215b8f97671b4  ./rb-sdk-cpp-0.11.10-aarch64-unknown-linux-gnu.tar.gz
ca0832cdbf1ef936906a72dda1a89c5ba53a4157af2f4ad181fc28668be72dff  ./rb-sdk-cpp-0.11.10-x86_64-unknown-linux-gnu.tar.gz
236c93ba4125a4e3a363adbc134c956cfc57e97fca69157dac57da2aa1acf22b  ./rb-sdk-cpp-0.11.10-x86_64-pc-windows-gnu.zip
```
