---
description: 유용한 시스템 설정을 알아봅니다.
image: /imgs/share.png
---

# 시스템 설정

설정해두면 유용한 시스템 설정을 알아봅니다. macOS Monterey를 기준으로 하였으나 다른 버전도 비슷비슷할 것으로 보입니다. 반드시 동일하게 설정할 필요는 없으며 보고 괜찮다 싶은 항목만 적용하세요.

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/system_preferences_main.png" alt="System Preferences" />
</div>

상단 메뉴의 `` 로고를 누르고 `System Preferences...`를 선택합니다.

:::tip 자동 설정 스크립트
하나하나 설정하기 귀찮으신 분은 [자동 설정 스크립트](./setting) 페이지를 참고해 주세요.
:::

## Dock & Menu Bar

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/dock_menubar.png" alt="Dock & Menu Bar" />
</div>

Dock을 자동으로 감추도록 설정합니다.

- `Dock & Menu Bar` > `Automatically hide and show the Dock`: 체크
- 좀 더 화면을 넓게 쓰기 위해서 Dock을 자동으로 감춥니다.
- 원래 Dock이 있던 화면 모서리로 커서를 가져가면 Dock이 나타납니다.

## 미션 컨트롤 <sup>Mission Control</sup>

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/mission_control.png" alt="Mission Control" />
</div>

미션 컨트롤 창 순서를 고정합니다.

- `Mission Control` > `Automatically rearrange Spaces based on most recent use`: 체크 해제
- 미션 컨트롤 창 순서가 기본적으로 최근 사용 순으로 설정되어 있어 의도하지 않게 순서가 변경되는 것을 막습니다.

## 언어 및 지역 <sup>Language & Region</sup>

<div class="image-600 no-radius">

![Language & Region](./imgs/index/language_region.png)

</div>

언어 설정을 영어 우선순위로 변경합니다.

- `Language & Region` > `Preferred languages`: 1. English > 2. 한국어 (드래그로 순서 조정)
- 간혹 locale 설정 때문에 오류가 발생하는 걸 방지해주고 영어 오류 메시지가 구글검색이 잘되는 편입니다.
- 특별히 문제가 없다면, 반드시 변경할 필요는 없습니다.

## 보안 <sup>Security & Policy</sup>

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/security_policy.png" alt="Security & Policy" />
</div>

패스워드를 잠자기 즉시 입력하도록 설정합니다.

- `Security & Privacy` > `General` > `Require password`: immediately
- 잠자기 모드나 화면 보호기가 켜지면 즉시 패스워드 입력을 활성화하여 보안을 최대한 안전하게 유지합니다.

분실대비 스크린 메시지를 설정합니다.

- `Security & Privacy` > `General` > `Show a message when the screen is locked`: 전화번호 / 이름
- 혹시 분실했을 경우를 대비하여 전화번호, 이름 등을 알려줍니다.

디스크 암호화를 활성화합니다.

- `Security & Privacy` > `FileVault`: Turn On FileVault
- 분실 시 복구 불가능하게 디스크를 암호화합니다.

## 키보드 <sup>Keyboard</sup>

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/keyboard_text.png" alt="Keyboard (Text)" />
</div>

모든 텍스트 자동 변경 옵션을 끕니다.

- `Keyboard` > `Text`: 모든 자동 변경 옵션 끄기
- 입력한 단어를 컴퓨터 마음대로 바꾸는 걸 방지합니다.
- 특히 Use smart quotes and dashes는 코드 복사하다가 따옴표가 바뀌면서 고생이 시작됩니다..

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/keyboard_shortcuts.png" alt="Keyboard (Shortcuts)" />
</div>

컨트롤 버튼(예, 아니오 등) 키보드로 제어하도록 설정합니다.

- `Keyboard` > `Shortcut` > `Use keyboard navigation to move focus between controls` : 체크함
- 예/아니오 버튼을 키보드로 선택할 수 있습니다.

## 트랙패트 <sup>Trackpad</sup>

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/trackpad.png" alt="Trackpad" />
</div>

클릭을 터치로 설정합니다.

- `Trackpad` > `Point & Click` > `Tab to click`: 체크함
- 트랙패드 클릭 시 꾸욱 누를 필요 없이 톡톡 터치로 클릭해서 손의 피로를 줄입니다.

## 접근성 <sup>Accessibility</sup>

<div class="image-600 no-radius">
  <custom-image src="/imgs/index/accessibility.png" alt="Accessibility" />
</div>

드래그를 세 손가락으로 가능하도록 설정합니다.

- `Accessibility` > `Pointer Control` > `Trackpad options...`: Enable dragging - three finger drag
- 창 또는 아이콘을 이동할 때 트랙패드를 누른 상태로 이동할 필요 없이 세 손가락으로 드래그 할 수 있습니다.
