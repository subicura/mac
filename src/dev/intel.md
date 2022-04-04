---
description: 패키지 관리자 설정 방법을 알아봅니다.
image: /imgs/share.png
---

# 패키지 관리자 (Intel)

:::warning Apple Silicon (M1)
이 페이지는 **Intel 사용자**를 대상으로 작성하였습니다.  
Apple Silicon (M1) 사용자는 [패키지 관리자 (Apple Silicon/M1)](./apple-silicon) 페이지를 확인하세요.
:::

`iTerm` 앱을 실행하고 개발 환경 구축을 위한 필수 프로그램을 설치합니다.

## Command Line Tools

macOS는 기본적으로 `gcc`, `make`와 같은 컴파일 도구가 설치되어 있지 않기 때문에 명령어 도구<sup>Command Line Tools</sup>를 설치해야 합니다. Xcode를 설치해도 되지만 iOS 개발을 할 게 아니라면 용량이 작은 명령어 도구만 따로 설치합니다.

**설치**

CLI에서 `gcc`나 `python` 같은 명령어를 입력하면 자동으로 다음과 같은 화면이 뜨고 `Install`을 선택하면 명령어 도구를 설치합니다.  
(iTerm 실행 시 설치했다면 skip!)

<div class="image-450 no-radius">
  <custom-image src="/imgs/intel/xcode-install.png" alt="XCode Install" />
</div>

수동으로 설치하려면 다음 명령어를 입력합니다.

```sh
xcode-select --install
```

**설치 확인**

```sh
# gcc test

$ gcc
clang: error: no input files
```

## Homebrew

brew<sup>homebrew</sup>는 각종 커맨드라인 프로그램과 일반 애플리케이션(크롬..)을 손쉽게 설치해주는 Mac용 패키지 매니저입니다. 리눅스의 `apt`나 `yum`과 비슷하며 다양한 프로그램을 복잡한 빌드과정 없이 손쉽게 설치하고 업데이트, 관리도 간단하므로 개발을 할 때 반드시 설치해야 하는 필수 프로그램입니다. `그냥 홈페이지 가서 다운로드 하고 설치하는 게 편한데..`라고 할 수 있지만, 나중에 업데이트나 삭제를 생각해보면 글쎄요.. brew 쓰세요!

**설치**

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

터미널을 재시작합니다.

**설치 확인**

```sh
# brew test
$ brew doctor
Your system is ready to brew.
```

## Git

버전 관리 도구로 유명한 git입니다. 다들 아시죠? macOS에 기본으로 설치되어 있지만, 최신 버전이 아니므로 brew를 이용해서 업데이트합니다. git-lfs 는 Git Large File Storage로 용량이 큰 바이너리 파일을 git으로 관리할 때 유용합니다. git 설치할 때 같이 설치합니다.

**설치**

```sh
brew install git git-lfs
```

git 설치가 완료되었으면 개인정보를 설정하고 맥에서 한글 파일명을 정상적으로 처리하기 위해 추가 옵션을 설정합니다. ~~망할 한글처리~~

**설정**

```sh
git lfs install
git config --global user.name "Your Name"
git config --global user.email "you@your-domain.com"
git config --global core.precomposeunicode true
git config --global core.quotepath false
```
