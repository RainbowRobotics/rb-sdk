# rainbow-rb-sdk

Rainbow Robotics C++ SDK(`librb_sdk`)를 배포하기 위한 APT 저장소 + 릴리스 아카이브 저장소입니다.
`main` 브랜치 자체에는 소스가 없고, 실제 패키지 저장소를 발행/관리하는 워크플로우와 서명 공개키만 있습니다.

## 설치 (Ubuntu / Debian, APT)

```bash
curl -fsSL https://rainbowrobotics.github.io/rb-sdk/rb-sdk-apt-repo.gpg.key \
  | sudo gpg --dearmor -o /usr/share/keyrings/rb-sdk-apt.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/rb-sdk-apt.gpg] https://rainbowrobotics.github.io/rb-sdk stable main" \
  | sudo tee /etc/apt/sources.list.d/rb-sdk.list
# arm64 환경이면 arch=arm64, 개발판이 필요하면 stable 대신 dev

sudo apt update
sudo apt install rainbow-rb-sdk-dev
```

특정 버전을 고정 설치하려면:

```bash
apt-cache madison rainbow-rb-sdk-dev
sudo apt install rainbow-rb-sdk-dev=1.2.3 rainbow-rb-sdk=1.2.3
# dev 채널: rainbow-rb-sdk-dev=1.2.3~dev4 rainbow-rb-sdk=1.2.3~dev4
```

## 다운로드 (GitHub Releases)

CI나 도커 빌드처럼 apt 없이 바이너리만 필요하면 [Releases](https://github.com/RainbowRobotics/rb-sdk/releases)에서
플랫폼별 tarball을 받아 쓰세요. (APT 트래픽은 GitHub Pages 대역폭 제한에 걸리므로, CI에서는 APT 대신 이 방법을 권장합니다.)

```bash
V=1.2.3
TRIPLE=x86_64-unknown-linux-gnu   # arm64: aarch64-unknown-linux-gnu
curl -fL "https://github.com/RainbowRobotics/rb-sdk/releases/download/$V/rb-sdk-cpp-$V-$TRIPLE.tar.gz" \
  | sudo tar -xzf - -C /usr/local
# CMake: find_package(rb_sdk PATHS /usr/local/lib/cmake/rb_sdk REQUIRED)
# pkg-config: PKG_CONFIG_PATH=/usr/local/lib/pkgconfig pkg-config --cflags --libs rb_sdk
```

> `librb_sdk.so.<version>`과 Python 패키지 `rainbow.rb_sdk`를 같은 프로세스에 함께 로드하지 마세요.

## 저장소 구성 (브랜치별 역할)

| 브랜치 | 역할 |
|---|---|
| `main` | 여기. `publish-apt-repo` 워크플로우와 저장소 서명 공개키(`rb-sdk-apt-repo.gpg.key`)만 관리 |
| `gh-pages` | GitHub Pages로 서빙되는 실제 APT 저장소 (`dists/`, `pool/`). 매 발행마다 통째로 재작성되는 orphan 브랜치 |
| `release/cpp/<version>` | 버전별 산출물(.deb 4종 + tarball 2종 + sha256)만 담은 보관용 orphan 브랜치. GitHub Release 태그가 이 브랜치를 가리키도록 재지정됨 |

APT 저장소 사이트: https://rainbowrobotics.github.io/rb-sdk/

## 배포 절차

배포는 `main`의 [`publish-apt-repo`](.github/workflows/publish-apt-repo.yml) 워크플로우(`workflow_dispatch`)로 이루어집니다.

1. GitHub Release에 4개의 `.deb`(런타임/dev × amd64/arm64)와 플랫폼별 tarball이 이미 올라가 있어야 합니다.
2. Actions 탭에서 `publish-apt-repo`를 실행하며 `version`(릴리스 태그), `channel`(`stable`/`dev`), `debver`(Debian 버전 문자열)를 입력합니다.
3. 워크플로우가 순서대로 수행합니다: 릴리스에서 `.deb`/tarball 다운로드 → `release/cpp/<version>` 브랜치에 산출물 커밋 및 릴리스 태그 재지정 → `gh-pages`의 `pool/`, `dists/` 갱신 및 GPG 서명 → Slack 알림.

서명 키 fingerprint: `605E 8364 5698 465E 1452 CBF0 C749 1A44 F2FB 92C6`
