# rb-sdk C++ SDK 0.11.11 (stable)

이 브랜치는 `0.11.11` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.11 rainbow-rb-sdk=0.11.11 rainbow-rb-zenoh-dev=0.11.11 rainbow-rb-zenoh=0.11.11
sudo apt install rainbow-rb-zenoh-dev=0.11.11 rainbow-rb-zenoh=0.11.11   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.11

## sha256
```
0a1888a58ffffb7df0d72167d235c00889ce09c821ca10dbf3f74df7d228beeb  ./rainbow-rb-sdk_0.11.11_amd64.deb
f87636b45e794548b12472b4d00a9d15e8af75e266553fb786117364842c1734  ./rainbow-rb-sdk_0.11.11_arm64.deb
a1e8f8b41c13b3e423a6b5c940a79270812efeb5cbc83d9f050fbd4fd7d50b93  ./rainbow-rb-sdk-dev_0.11.11_amd64.deb
4de5d5197f001aed55b6d46c34030c1d9f21a5591f3468a7f64694530ec5a596  ./rainbow-rb-sdk-dev_0.11.11_arm64.deb
c7b88918a637e0d251861813fba40be50817839b45baaeb14d4a2393ee666b72  ./rainbow-rb-zenoh_0.11.11_amd64.deb
e4f08861d9f4a7bf3696702a302eb99fecc29014f2c78e155d75d2d49efd0316  ./rainbow-rb-zenoh_0.11.11_arm64.deb
543e01af55ff4dc8bb03fbd5c75e3360b8b9058223626157438b5cbf6b95ce8b  ./rainbow-rb-zenoh-dev_0.11.11_amd64.deb
c9cf6d5270702b59b442f04f8fab8347ec360b2d6c8525e2a6a61e1ad6a858e1  ./rainbow-rb-zenoh-dev_0.11.11_arm64.deb
1ac8243f61d9230652de572e99ac43004a740ebbccf11dd6743942a3d70f908d  ./rb-sdk-cpp-0.11.11-aarch64-unknown-linux-gnu.tar.gz
405cc2d67857fd95399beb9ab3dd7d664d152c33546fa33ea10153e35fa5fb11  ./rb-sdk-cpp-0.11.11-x86_64-unknown-linux-gnu.tar.gz
f44859bc7f241ae99e94f3d0187168fb6d8f2d74ed019698425c26e0819f667b  ./rb-sdk-cpp-0.11.11-x86_64-pc-windows-gnu.zip
```
