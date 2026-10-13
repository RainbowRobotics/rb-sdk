# rb-sdk C++ SDK 0.10.1 (stable)

이 브랜치는 `0.10.1` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.1
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.1

## sha256
```
f79cf79de4df9884ee4dd24dc03582cea98f3cdd768d7f99283f6609c16af5b7  ./rainbow-rb-sdk_0.10.1_amd64.deb
1c58c2ac524d72d9687510e0dfbfc69f674d088928f8c91bbfeb586b48abe34e  ./rainbow-rb-sdk_0.10.1_arm64.deb
bd9d6265a3cf1f278bb7f75e7a544b156f033a93ccb6643ca8375291216d54f0  ./rainbow-rb-sdk-dev_0.10.1_amd64.deb
27b3290d5d3e299124b015f01cc27d01c5d6e7aac12b7d6b374a6decfdfa45be  ./rainbow-rb-sdk-dev_0.10.1_arm64.deb
a707d242b23ee220c332e22f7c023d731b5585e9cee0c530a36cd03a38177b46  ./rb-sdk-cpp-0.10.1-aarch64-unknown-linux-gnu.tar.gz
a5a3ae16c2cabbcc724ce12f118111640e125396ebe6e0b0c87f86a1d40a3e72  ./rb-sdk-cpp-0.10.1-x86_64-unknown-linux-gnu.tar.gz
3c2fbd7927b6e3301043671569d7897b94dd959c16e0738be9ad94e61b985271  ./rb-sdk-cpp-0.10.1-x86_64-pc-windows-gnu.zip
```
