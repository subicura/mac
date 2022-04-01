---
description: macOS의 장점과 단점을 알아봅니다.
image: /imgs/share.png
---

# macOS 특징

본격적인 설명에 앞서 Windows와 비교하여 macOS의 장점과 단점을 알아봅니다.

:::tip 요약

- **장점**: 애플 생태계, 이쁘고, 터미널 좋고 편하고 M1 가성비 좋음
- **단점**: 게임, 문서, 공공기관, GPU 관련 작업 어렵고 자잘한 한글, 모니터, 마우스 등 호환성 이슈와 A/S 비용이 비쌈

:::

## macOS의 장점

**애플**

<custom-image src="/imgs/macos-vs-windows/apple_logo.png" alt="Apple" />

- 애플이 만듦 ~~스타벅스 출입 가능~~
- iPhone, iPad, Apple Watch 연동
  - 별도 프로그램 설치 없이 기본으로 [연속성 기능](https://support.apple.com/ko-kr/HT204681) 제공
  - [Handoff](https://support.apple.com/ko-kr/HT209455), [공통클립보드](https://support.apple.com/ko-kr/HT209460), [iPhone 셀룰러 통화](https://support.apple.com/ko-kr/HT209456), [문자 메시지 전달](https://support.apple.com/ko-kr/HT208386), [Instant Hotspot](https://support.apple.com/ko-kr/HT209459) 등
  - 애플 생태계로 묵이면 사용하기 짱짱 편함 ~~폐쇄성~~

**디자인**

![macOS HIG](./imgs/macos-vs-windows/macOS_HIG.svg)

- 일관되고 직관적인 UI - [Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/macos/overview/themes/)
  - 거의 완벽하게 [다크 모드를 지원](https://developer.apple.com/design/human-interface-guidelines/macos/visual-design/dark-mode/)하고 써드파티 지원도 훌륭함
- 한글 폰트 가독성 좋음 ~~Windows 맑은 고딕도 바뀔 때가 됐는데..~~
- 👁 레티나<sup>Retina</sup> 디스플레이와 HiDPI 지원으로 선명한 화면 제공

**개발 환경**

<div class="image-600 no-radius">

<custom-image src="/imgs/macos-vs-windows/neofetch.png" alt="neofetch" />

</div>

- macOS를 지원하는 게임이 적어 개발에 집중할 수 있음 🤔
- 유닉스 계열에서 오는 장점
  - 터미널 사용이 편안 (bash, zsh 기본 사용)
  - 각종 개발 도구 사용 및 라이브러리 설치 편안
  - 환경변수 설정 편안
  - Windows에서 최신 언어나 프레임워크를 사용하려면 보통 시간이 더 걸리고 뭔가(?) 복잡한 경우가 많음 ~~Windows에서 Ruby on rails를 설정해보자!~~
- 많은 오픈소스 개발자가 맥 또는 리눅스 사용
  - 외국 컨퍼런스를 가면 이상하게(?) 맥을 많이 씀. 맥 또는 리눅스?
  - 개발환경 자체가 유닉스 환경에 최적화되어 있는 경우가 많음
- iOS 개발 가능

**편의성**

<div class="image-300 no-radius">

<custom-image src="/imgs/macos-vs-windows/trackpad2-mission-control.png" alt="TrackPad Gensture" />

</div>

- 쫀득한 트랙패드와 훌륭한 멀티터치 제스처
  - Windows 노트북의 그것과는 다름
- Touch ID 통합 완성도
- 맥북 모니터를 닫으면 자동으로 Sleep 모드 진입
  - 일반적으로 거의 전원을 끄지 않고 사용함
- 오래 써도 시스템이 많이 느려지지 않음 ~~느려지니까 한번 밀까? 이런 거 없음~~
- 보안 및 개인정보 강화
  - OS 자체에서 앱별 접근 권한 제어
  - Windows보다 바이러스가 적음. ~~운영체제 인기가 없어서..~~
  - 하지만 비밀번호 없이 root 계정 로그인이 가능한 어이없는 결함도 생김. 보안은 항상 조심

**가성비**

- 예전엔 비싼게 단점이였는데, M1 등장 후 가성비 압승
  - Apple 교육 할인 스토어에서 MacBook Air 최저 1,160,000원
  - M1 - 가격은 Air, 성능은 Pro 급

**전용앱**

- 로직(Logic), 파이널 컷(Final Cut) 등 꽤 괜찮은 macOS 전용 음악 편집, 영상 편집 프로그램
- 음악 작업 시 macOS를 사용하는 경우가 많음

## macOS의 단점

**Windows 지원**

- IE(Internet Explorer) 테스트 어려움
- 대부분 인기 게임은 Windows 용으로 나옴 ~~LOL은 됨~~
- 오피스(워드, 엑셀, 파워포인트), 한글 워드 프로세스 지원 어려움. 최근 마이크로소프트에서 macOS용 오피스 프로그램에 신경을 많이 쓰고 있음
- 최근 많이 개선되긴 했으나.. 관공서 업무시 Windows 필수 ~~2023년쯤이면 거의 해결되지 않을까..?~~

**개발 환경**

- GPU 약함. 애초에 조립PC를 지원하지 않으므로 원하는 그래픽카드 사용이 어려움
- AMD 그래픽 카드를 밀면서 NVIDIA CUDA 지원 안 됨
- GPU 관련 머신러닝 작업 어려움

**한글 지원**

- 한/영 전환 딜레이 🤬 [👉 딜레이 없애는 방법 알아보기](../setup/hangle-input.html#한-영-전환을-빠르게)
- 한글 입력 이슈
  - 마지막 입력한 글자가 잘리거나, 자모가 분리되거나..
  - Windows에서 자모가 분리되는 한글 파일명. ex) `ㅎㅏㄴㄱㅡㄹ.txt`

**편의성**

- 마우스 사용 불편. 트랙패드에 최적화되어 있음
- 모니터 호환성. HiDPI 지원이 제대로 안 되는 모니터가 있음.
- 🔥 발열 이슈. 5분만 사용해도 뜨거움. 하지만 M1이라면??
- 폐쇄적. 벽돌이 되거나 문제가 생겼을 때 개인 조치 불가

**가성비**

- M1이 저렴하지만, 추가 메모리나 악세서리는 아직도 비쌈
- 쓸만한 앱들이 유료가 많아 앱 구매 비용 비쌈
- 문제가 생기면 따로 조치하기가 어려워 A/S 비용 비쌈
