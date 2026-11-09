# SwitchMac 베타 내려받기

Windows 11을 Mac처럼 바꿔 주는 무료 프로그램 **SwitchMac**의 베타 설치 파일을 모아 두는 곳이에요. 소스 코드는 여기 없어요.

- **내려받기:** 오른쪽 **Releases**에서 가장 위 버전의 `SwitchMac-Setup-*.exe`
- **필요한 것:** Windows 11 22H2 이상
- **설치 방법과 Windows 경고가 뜨는 이유:** 릴리스에 같이 올린 `install-guide-ko.txt`(설치 안내)

## 받은 파일이 진짜인지 확인하기

설치 전에 PowerShell에서 아래처럼 확인할 수 있어요. 같이 올린 `verify-setup.ps1`과 `.miri-sig`를 설치 파일과 같은 폴더에 두세요.

```powershell
powershell -ExecutionPolicy Bypass -File verify-setup.ps1 SwitchMac-Setup-0.1.0-beta.exe -Fingerprint 222A-F6C3-9D43-6FAF-F532
```

"서명이 맞고, 열쇠 지문도 알려 준 값과 같습니다"라고 나오면 만든 사람이 만든 그대로의 파일이에요. 만든 사람 확인 열쇠 지문은 **222A-F6C3-9D43-6FAF-F532** 입니다.

이 확인은 파일이 바뀌지 않았다는 뜻이에요. Windows의 "알 수 없는 게시자" 경고를 없애 주지는 않아요.

## 의견 보내기

인스타그램 [@switch_mac_kr](https://www.instagram.com/switch_mac_kr/)

만든 사람: 미리(miri)
