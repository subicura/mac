# 자동 설정 스크립트

macOS는 각종 설정을 보통 `~/Library/Preferences` 폴더에 `.plist` 파일로 관리합니다. 시스템 및 파인더 설정도 동일한 방식을 사용하고 `defaults` 명령어로 설정할 수 있기 때문에 스크립트로 자동화 할 수 있습니다.

## 스크립트 실행

터미널을 열고 다음 명령어를 입력하여 [시스템 설정](./index)과 [파인더 설정](./finder)에 나온 대부분의 내용을 한 번에 설정할 수 있습니다.

```sh
/bin/zsh -c "$(curl -fsSL https://raw.githubusercontent.com/subicura/settings/main/macos/system_setting.zsh)"
```

<asciinema id="setting_script" title="setting script" src="/mac/asciinema/setting-script.cast" />

::: tip
스크립트 설정 후 반드시 시스템을 재시작해야 변경사항이 적용됩니다. 사용한 스크립트는 [여기서](https://github.com/subicura/settings/blob/main/macos/system_setting.zsh) 확인하세요.
:::

## 추가 설정

안타깝게도 ~~;ㅁ;~~ 모든 설정을 스크립트로 지정할 수 없어, 일부 설정은 추가로 수동 설정해야 합니다.

- [시스템 설정 - 언어 및 지역](./#언어-및-지역-language-region)
- [시스템 설정 - 보안](./#보안-security-policy)
- [파인더 설정 - 다운로드 폴더 옵션](./finder.html#다운로드-폴더-옵션)
