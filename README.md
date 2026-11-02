# rb-sdk C++ SDK 0.11.1 (stable)

이 브랜치는 `0.11.1` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.1
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.1

## sha256
```
e34eac722ed1f44d0cabe33bbcbb250abfa09e8651ee4aaf35821bc2f25bcccb  ./rainbow-rb-sdk_0.11.1_amd64.deb
c52b7a5550d02956b0acf1e9596bc1d65bc80c5af223a6ab4a52abb6d80309a3  ./rainbow-rb-sdk_0.11.1_arm64.deb
f6013f99548e1d3d10b14c0abd970ff3558b1d941c940628b67b756e19243314  ./rainbow-rb-sdk-dev_0.11.1_amd64.deb
ea8d1fc25bb939cc3d7c266bf2c1e81b749558088e2ddcee75f8c7c95d9f4efe  ./rainbow-rb-sdk-dev_0.11.1_arm64.deb
53db6c1aeec322fa05870e8c908752dbe320a01ca235ff475b41f975d4c1dab0  ./rb-sdk-cpp-0.11.1-aarch64-unknown-linux-gnu.tar.gz
3f9814dcfa706e13d5e622a04d99c03f58e0d3ca6fd666a1830844fb3f04bac0  ./rb-sdk-cpp-0.11.1-x86_64-unknown-linux-gnu.tar.gz
b3ec37cfee634103568d9f28afc1ae55cea87c8c51b55fbefe5113453e50ad1a  ./rb-sdk-cpp-0.11.1-x86_64-pc-windows-gnu.zip
```
