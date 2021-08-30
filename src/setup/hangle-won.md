---
description: 한글 관련 설정을 알아봅니다.
image: /imgs/share.png
---

# `₩` 입력 개선

macOS는 한글입력 일 땐 `₩`가 입력되고 영문입력 일 땐 `` ` ``가 입력되어 불편한 경우가 많습니다. 무조건 `` ` ``가 입력되도록 시스템을 설정합니다. `₩`를 입력하려면 한글 입력 상태에서 `⌥(Options)`과 함께 입력합니다.

## `₩` 대신 `` ` `` 입력하기

**~/Library/KeyBindings/DefaultkeyBinding.dict**

해당 위치에 파일을 생성하고 다음과 같은 내용을 입력합니다.

```sh
{
  "₩" = ("insertText:", "`");
  "~₩" = ("insertText:", "₩");
}
```

또는 터미널을 열고 다음 명령어를 복붙합니다.

```sh
mkdir ~/Library/KeyBindings

cat <<EOF > ~/Library/KeyBindings/DefaultkeyBinding.dict
{
  "₩" = ("insertText:", "\`");
  "~₩" = ("insertText:", "₩");
}
EOF
```

OS 재시작이 필요합니다.
