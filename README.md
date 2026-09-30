# rb-sdk C++ SDK 0.1.4 (stable)

이 브랜치는 `0.1.4` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.4
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.4

## sha256
```
a5f03d52f0acd97c6103e901b33c1602d784d47fba8bb4f352363df7d93ad82d  ./rainbow-rb-sdk_0.1.4_amd64.deb
9a080b3f77dbd0049cf6780977274cd5b5814ae2463ebb4f5da7d2120caaf2fd  ./rainbow-rb-sdk_0.1.4_arm64.deb
274eff7be038812dcb40f34f9198d6004d8957149bcc1d6022956cc25e81b200  ./rainbow-rb-sdk-dev_0.1.4_amd64.deb
973aee73da821a1c4fe98b9f81cad5ecafc30c7f3d76055c8e9f672f6779f043  ./rainbow-rb-sdk-dev_0.1.4_arm64.deb
9a4a8474c9cf0fa9ef530d80df2290d28dc79b6524c7618f243029c2dfbb8f9b  ./rb-sdk-cpp-0.1.4-aarch64-unknown-linux-gnu.tar.gz
9a6b45335f07d81c0e42eec50a90d42b795d937aa7cf3934f4ffd008eeeb7578  ./rb-sdk-cpp-0.1.4-x86_64-unknown-linux-gnu.tar.gz
11e04a0e2dea981a035b9d98b135b086804bc737cb05f63f52375274311d660e  ./rb-sdk-cpp-0.1.4-x86_64-pc-windows-gnu.zip
```
