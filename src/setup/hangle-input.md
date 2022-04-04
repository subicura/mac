---
description: 한영 키보드 전환을 빠르게 하는 방법을 알아봅니다.
image: /imgs/share.png
---

# 한/영 전환

macOS의 기본 한/영 전환은 `CapsLock(한/A)`키 또는 `⌃(Ctrl)` + `Space` 입니다. 문제는 가끔 전환 딜레이가 있어 의도치 않게 한글 또는 영어가 입력되는 경우가 많다는 점입니다. 🤬🤯

## 한/영 전환을 빠르게

완벽하진 않지만, 딜레이 문제를 해결하는 방법이 있습니다.

1. 키 맵핑 프로그램 설치
2. `Caps Lock`을 `F19`(사용하지 않는 키)로 맵핑
3. Input Source 전환 키를 `F19(=Caps Lock)`로 설정

### Karabiner-Element 설치

키 맵핑 프로그램으로 `Karabiner-Element`를 사용합니다.

<div class="image-600">
  <custom-image src="/imgs/hangle/install-01.jpg" alt="Apple Beta Software" />
</div>

1. [홈페이지](https://karabiner-elements.pqrs.org/)에서 프로그램을 다운로드 합니다.

<div class="image-600">
  <custom-image src="/imgs/hangle/privacy-tab.png" alt="Apple Beta Software" />
</div>

2. 전체 키 입력을 받기 때문에 보안 설정이 까다롭습니다. 각종 보안 설정을 허용합니다.

<custom-image src="/imgs/hangle/karabiner-element.png" alt="Karabiner Element" />

3. `caps_lock`을 `F19`로 설정합니다. 이제 `Caps Lock` 키를 누르면 `F19`가 눌리게 됩니다.

<div class="image-600">

<custom-image src="/imgs/hangle/input-source-key.png" alt="Input Source" />

</div>

4. `System Preferences...` > `Keyboard` > `Shortcuts` > `Input Source`에서 `Select next source in Input menu` 단축키를 `F19`로 설정하면 완료!
