# rb-sdk C++ SDK 0.10.5 (stable)

이 브랜치는 `0.10.5` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.5
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.5

## sha256
```
f8df8998a25438df254a75d864322d872e524c8d7acad5ffd573d2fc169db796  ./rainbow-rb-sdk_0.10.5_amd64.deb
ca57eee543f3b3cfb3d9bd139b448037fa5fda4b6b21a9438f8b5360d07d872d  ./rainbow-rb-sdk_0.10.5_arm64.deb
3f12d34f056d3be84e2e685a1bb9da9d1030feecf95c64eb3f3a73920c9fd541  ./rainbow-rb-sdk-dev_0.10.5_amd64.deb
4986ad417b795a14cecb12b8b6dfbd6f463f3aecff764b276dd6ceb279beff72  ./rainbow-rb-sdk-dev_0.10.5_arm64.deb
8285ae72f31afc4fea2baf5f455e7060188d353a6ce71cc801d283a16e2ce3c1  ./rb-sdk-cpp-0.10.5-aarch64-unknown-linux-gnu.tar.gz
191baa1a2d797dc37313528be0a56d3524adeb8ef7714f8edc9253a149d0e754  ./rb-sdk-cpp-0.10.5-x86_64-unknown-linux-gnu.tar.gz
47756d205d99d29ae2a36034452af84be0d11325741b8009a5cb88f0c9840bf0  ./rb-sdk-cpp-0.10.5-x86_64-pc-windows-gnu.zip
```
