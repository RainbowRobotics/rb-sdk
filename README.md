# rb-sdk C++ SDK 0.11.13 (stable)

이 브랜치는 `0.11.13` 배포 산출물 보관용입니다 (apt 저장소 아님).
설치는 gh-pages APT 저장소를 쓰세요:

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg
echo 'deb [signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main' | sudo tee /etc/apt/sources.list.d/rb-sdk.list
sudo apt update && sudo apt install rainbow-rb-sdk-dev=0.11.13 rainbow-rb-sdk=0.11.13 rainbow-rb-zenoh-dev=0.11.13 rainbow-rb-zenoh=0.11.13
sudo apt install rainbow-rb-zenoh-dev=0.11.13 rainbow-rb-zenoh=0.11.13   # zenoh 클라이언트만 필요할 때
```

- release: https://github.com/RainbowRobotics/rb-sdk/releases/tag/0.11.13

## sha256
```
a2bd3ed02fdf06f59b81a04b6bb168846d71a3f91a7dd140f9c76bf8d9750fd6  ./rainbow-rb-sdk_0.11.13_amd64.deb
ea9545747d10950f705472e1fd5314609d43d85ba1ed6e3c997d357c0dd55d61  ./rainbow-rb-sdk_0.11.13_arm64.deb
059b819decf6302b94f44afaaa9f25eaf473f9f0ac18db1456066fa2886254fc  ./rainbow-rb-sdk-dev_0.11.13_amd64.deb
d9d45bc10f98ac40e22a88d3c44d3656742c7b99a3c40bfa89efe99da264e7ff  ./rainbow-rb-sdk-dev_0.11.13_arm64.deb
deefef5ffbbec303ed4a2fee579d54f6652465c5d15d145ec9857f366c45d752  ./rainbow-rb-zenoh_0.11.13_amd64.deb
b80f3e01b91a24b536f1149846b55591e4719ceac9a9c2f34e8b329b54729332  ./rainbow-rb-zenoh_0.11.13_arm64.deb
beffead5d46bb4343b3647818fdfcef30584d53172c961a061f529869930a682  ./rainbow-rb-zenoh-dev_0.11.13_amd64.deb
c338b282fe2c31fc8bde933dae649a89da4096f62ab635bcea8b9e896bef4eed  ./rainbow-rb-zenoh-dev_0.11.13_arm64.deb
45fee03a2315962868a0c9b279a29d69a89ad6378c0a44bfab52f158f9c13ad6  ./rb-sdk-cpp-0.11.13-aarch64-unknown-linux-gnu.tar.gz
ed769c91db733ce7d0c810ee3633449de642ef120bcc98cd7ffdce8f983c9a14  ./rb-sdk-cpp-0.11.13-x86_64-unknown-linux-gnu.tar.gz
eb335948034ee4247f4c4f20d304533cc013e84244605fda155a14decb46f8a5  ./rb-sdk-cpp-0.11.13-x86_64-pc-windows-gnu.zip
```
