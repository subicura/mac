---
description: macOS에 Windows를 설치하는 방법을 소개합니다.
image: /imgs/share.png
---

# Windows 설치

macOS에서 Windows를 사용하는 방법은 처음부터 부팅을 다르게 하는 `Boot Camp`와 가상화 프로그램을 설치하여 macOS와 Windows를 동시에 사용할 수 있는 `Parallels`, `VMWare Fusion`가 있습니다.

Windows를 설치하기 위해선 Windows 10 ISO 파일이 필요합니다. [여기서](https://www.microsoft.com/ko-kr/software-download/windows10ISO) 다운로드 하세요.

::: warning Apple Silicon
Boot Camp는 `Intel`기반 Mac에서만 사용할 수 있고, `Parallels`를 사용하면 `Apple Silicon`에서도 `ARM`기반 Windows를 설치할 수 있습니다.
:::

## Boot Camp <Badge text="무료"/>

`Boot Camp`는 `Intel`기반 macOS에 기본으로 포함되어 있는 기능입니다.

**Window 설치**

<custom-image src="/imgs/windows/bootcamp-01.png" alt="Boot Camp" />

1. `Applications` > `Utilities` > `Boot Camp Assistant` 실행

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/bootcamp-02.png" alt="Boot Camp" />
</div>

2. `Continue` 선택

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/bootcamp-03.png" alt="Boot Camp" />
</div>

3. Windows 10 ISO를 미리 다운받고 파티션 용량을 조절

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/bootcamp-04.png" alt="Boot Camp" />
</div>

4. 설치 후 재부팅

**드라이버 설치**

<div class="image-450">
  <custom-image src="/imgs/windows/bootcamp-windows.png" alt="Boot Camp" />
</div>

1. 재부팅 후 관련 드라이버 설치

**Windows 부팅**

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/bootcamp-05.png" alt="Boot Camp" />
</div>

1. 시동 디스크 선택하거나 부팅 후 `⌥(Option)`키를 입력하여 부팅 디스크 선택

## Parallels <Badge text="유료"/>

<div class="image-300 no-radius">
  <custom-image src="/imgs/windows/parallels.png" alt="Parallels" />
</div>

[홈페이지](https://www.parallels.com/)에 접속하여 Parallels를 다운로드합니다.

<custom-image src="/imgs/windows/parallels-download.png" alt="Parallels" />

1. `DOWNLOAD FREE TRIAL` 선택

## VMWare Fusion <Badge text="무료/유료"/>

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/vmware.png" alt="VMWare Fusion" />
</div>

VMWare Fusion Player는 개인용은 무료로 제공합니다. 무료로 키를 받고 설치하는 과정을 알아봅니다.

**무료 라이선스 키 발급**

<custom-image src="/imgs/windows/vmware-01.png" alt="VMWare Fusion" />

1. [홈페이지](https://www.vmware.com/products/fusion.html) 접속 후, `REGISTER TO GET YOUR KEY NOW` 선택

<custom-image src="/imgs/windows/vmware-02.png" alt="VMWare Fusion" />

2. 회원가입

<custom-image src="/imgs/windows/vmware-03.png" alt="VMWare Fusion" />

3. 다운로드 및 라이선스 키 확인

<div class="image-600 no-radius">
  <custom-image src="/imgs/windows/vmware-04.png" alt="VMWare Fusion" />
</div>

4. VMWare Fusion 설치시 라이선스 키 입력
