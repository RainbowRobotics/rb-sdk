# rb-sdk C++ SDK 0.1.5 (stable)

이 브랜치는 `0.1.5` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.1.5
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.1.5

## sha256
```
e1f9c01cb796d64a4b075072d5362225003a6430d7e7bedcfaad760c09b14f4d  ./rainbow-rb-sdk_0.1.5_amd64.deb
4ca59f9c7bade50e8fa8bb0346cf5c84b76da9451e84039f38427e8bd0bd2632  ./rainbow-rb-sdk_0.1.5_arm64.deb
f6ee36b0deff6077580da201013157290a4673e112945cbe4bc02a9b10fc9c2d  ./rainbow-rb-sdk-dev_0.1.5_amd64.deb
3a817fc77eee7386a10e1e3e91cfc403b91bb63171618ee285e44ea755e830e9  ./rainbow-rb-sdk-dev_0.1.5_arm64.deb
b22071ca92f893374354005bcbf4361c5af7537fd493d06d4e8386fa5681e6b9  ./rb-sdk-cpp-0.1.5-aarch64-unknown-linux-gnu.tar.gz
d1d00ff876d3fe235fbf8a0bba5403b170c55b2c0cce8d385967b86d52dd354a  ./rb-sdk-cpp-0.1.5-x86_64-unknown-linux-gnu.tar.gz
a34de2dc038f16406275feb242640b124cb92004c34ca0ee07188ab5fea30ec2  ./rb-sdk-cpp-0.1.5-x86_64-pc-windows-gnu.zip
```
