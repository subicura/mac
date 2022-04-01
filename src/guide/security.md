---
description: macOS 보안에 대해 알아봅니다.
image: /imgs/share.png
---

# 보안

macOS는 앱을 실행 할 때 세부적인 권한을 체크합니다.

## 설치 확인

<div class="image-350 no-radius">

<custom-image src="/imgs/security/open.jpg" alt="Open" />

</div>

다운로드받은 앱은 최초 1회 경고합니다. `Open`을 선택하면 앱이 열립니다.

:::warning 주의
경고만 뜨고 `Open` 버튼이 없는 경우, 주의가 필요한 앱이라는 의미입니다. 확실히 문제가 없다고 판단되면 오른쪽 버튼을 누르고 앱을 명시적으로 실행합니다. 그럼 `Open` 버튼이 노출됩니다.
:::

## 보안

<div class="image-350 no-radius">

<custom-image src="/imgs/security/block-popup.png" alt="Blocked Allow" />

</div>

특별한 권한을 요구하는 앱은 `Security & Privacy`에서 허용이 필요합니다.

<div class="image-600 no-radius">

<custom-image src="/imgs/security/blocked.png" alt="Blocked Allow" />

</div>

`Security & Privacy` > `General` 탭에서 하단 `Allow` 버튼을 선택합니다.

## 세부 권한

폴더에 접근하거나, 카메라를 사용하거나, 마이크를 사용하는 등 세부적인 권한이 필요하면 단순히 `OK`로 허용하는 경우가 있고 `Security & Privacy` > `Privacy` 탭에서 체크해야 하는 경우가 있습니다.

<div class="image-350 no-radius">

<div>
  <custom-image src="/imgs/security/access.png" alt="Access" />
</div>

<div>
  <custom-image src="/imgs/security/camera.png" alt="Camera" />
</div>

<div>
  <custom-image src="/imgs/security/microphone.png" alt="Microphone" />
</div>

</div>

<div class="image-450 no-radius">

<custom-image src="/imgs/security/open-security.png" alt="Open Security" />

</div>

<div class="image-600 no-radius">

<custom-image src="/imgs/security/privacy-tab.png" alt="Privacy" />

</div>

## 알림 확인

<div class="image-350 no-radius">

<custom-image src="/imgs/security/notification.png" alt="Notification" />

</div>

알림을 보내는 앱은 추가로 알림 권한을 요청합니다.
