# rb-sdk C++ SDK 0.10.3 (stable)

이 브랜치는 `0.10.3` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.10.3
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.10.3

## sha256
```
c736e1103a1090a5f88f638a8347cda2a2679cbedf1a5312b929e296d2dfae1a  ./rainbow-rb-sdk_0.10.3_amd64.deb
6028058a380f2f2d4fd8ab8608bda3abc396b8547b56e5e8586c6352db24e27d  ./rainbow-rb-sdk_0.10.3_arm64.deb
602666b7ca64d670b8c53894e08e802e74e80d9694296adfb6939ce7c2398a6c  ./rainbow-rb-sdk-dev_0.10.3_amd64.deb
29ff82267e7da19b57c11456d29d58fdf188a0476103da051f814353bec9d6e8  ./rainbow-rb-sdk-dev_0.10.3_arm64.deb
3adf7b137e495e49be243204fed2aa14b7031521c5d787c2a69c1c0470b2de58  ./rb-sdk-cpp-0.10.3-aarch64-unknown-linux-gnu.tar.gz
60837dfab2edfaf4f6ed4cbe3ca2184f30d277b0f7e568a426ab52cc96c97a6c  ./rb-sdk-cpp-0.10.3-x86_64-unknown-linux-gnu.tar.gz
30292c444ba4363f2ec9fa4a03783c3e5f88590765580944f357d2ee7b183222  ./rb-sdk-cpp-0.10.3-x86_64-pc-windows-gnu.zip
```
