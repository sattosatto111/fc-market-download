# 이적시장 분석 앱 설치 안내

## 갤럭시 (안드로이드)
1. 폰에서 [fc_market.apk](https://github.com/sattosatto111/fc-market-download/releases/latest/download/fc_market.apk) 를 받는다.
2. 받은 파일을 누르면 설치된다. "출처를 알 수 없는 앱 허용"을 물으면 허용.

## 아이폰
아이폰은 앱 파일을 눌러서 설치할 수 없다. PC에서 본인의 무료 Apple ID로 서명해 USB로 넣어야 하는데, 그 과정을 **아이폰설치.exe** 하나가 다 해 준다.

### 준비물
- Windows PC, USB 케이블, 아이폰(iOS 16 이상), 본인 Apple ID(무료 계정이면 됨)
- PC에 **iTunes** (USB 드라이버 때문에 필요). 없으면 프로그램 안의 [iTunes 설치] 버튼으로 넣는다.

### 순서
1. [아이폰설치.exe](https://github.com/sattosatto111/fc-market-download/releases/latest/download/iphone_install.exe) 를 받아 실행한다. (Windows가 "알 수 없는 게시자" 경고를 띄우면 '추가 정보 → 실행')
2. 아이폰을 USB로 PC에 연결하고 잠금을 푼 뒤, 아이폰에 "이 컴퓨터를 신뢰"를 누른다. 프로그램 위쪽 두 줄이 ✔ 가 되면 준비 끝.
3. Apple ID와 비밀번호를 넣고 **[아이폰에 설치]**. 아이폰에 6자리 인증 코드가 뜨면 프로그램에 넣는다. (입력은 애플 서버로만 간다. 서명은 오픈소스 Sideloader가 한다.)
4. 끝나면 아이폰에서:
   - 설정 → 개인정보 보호 및 보안 → **개발자 모드** 켜기 (재시동됨)
   - 설정 → 일반 → VPN 및 기기 관리 → 본인 Apple ID 프로필 **신뢰**

### 알아둘 것
- 무료 Apple ID 서명은 **7일** 뒤 만료된다. 그때 아이폰설치.exe를 다시 실행하면 된다(1분).
- PC 없이 폰에서 갱신하고 싶으면 프로그램 아래의 "SideStore 설치"를 쓴다. 그 뒤 폰에서 WireGuard 설치·sidestore.io 설정 파일 켜기·SideStore 로그인 → Refresh All, Sources에 아래 주소 추가 → Browse에서 이적시장 분석 Install.
  ```
  https://raw.githubusercontent.com/sattosatto111/fc-market-download/main/source.json
  ```
- 무료 계정은 이렇게 넣은 앱을 3개까지만 둘 수 있다.
- 막히면 가장 흔한 원인: iTunes 미설치(아이폰이 안 보임), 아이폰에서 "신뢰"를 안 누름, 개발자 모드 꺼짐(앱이 안 열림).
