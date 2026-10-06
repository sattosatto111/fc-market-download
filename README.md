# 이적시장 분석 앱 설치 안내

## 갤럭시 (안드로이드)
1. 폰에서 [fc_market.apk](https://github.com/sattosatto111/fc-market-download/releases/latest/download/fc_market.apk) 를 받는다.
2. 받은 파일을 누르면 설치된다. "출처를 알 수 없는 앱 허용"을 물으면 허용.

## 아이폰
아이폰은 앱 파일을 눌러서 설치할 수 없어서, 무료 Apple ID로 서명해 주는 **SideStore**를 먼저 넣어야 한다. 처음 한 번만 PC가 필요하고, 그 뒤로는 폰만으로 설치·갱신이 된다.

### 준비물
- Windows PC, USB 케이블, 아이폰(iOS 16 이상), 본인 Apple ID(무료 계정이면 됨)
- PC에 **iTunes** 설치 (Microsoft Store에서 무료). USB 드라이버 때문에 꼭 필요하다.

### PC에서 할 일 (한 번만)
1. [아이폰설치도구.zip](https://github.com/sattosatto111/fc-market-download/releases/latest/download/iphone_tools.zip) 을 받아 압축을 푼다.
2. 아이폰: 설정 → 개인정보 보호 및 보안 → **개발자 모드** 켜기 (재시동됨).
3. 아이폰을 USB로 PC에 연결하고 아이폰에 "이 컴퓨터를 신뢰" 누르기.
4. 압축 푼 폴더의 **`1_PC에서_실행.bat`** 을 더블클릭한다.
   - 검은 창에서 Apple ID, 비밀번호, 2단계 인증 코드를 묻는다. 입력은 애플 서버로만 간다(SideStore·Sideloader는 오픈소스).
   - 끝나면 아이폰에 SideStore 앱이 생기고, 페어링 파일이 아이폰으로 전송된다(공유 창이 뜨면 SideStore로 저장).

### 아이폰에서 할 일
1. 설정 → 일반 → VPN 및 기기 관리 → 본인 Apple ID 프로필 **신뢰**.
2. App Store에서 **WireGuard** 앱 설치.
3. 사파리로 https://sidestore.io 에 들어가 WireGuard 설정 파일을 받아 WireGuard 앱에 넣고 **켠다**.
4. SideStore 앱 열기 → PC에서 쓴 것과 같은 Apple ID로 로그인 → Apps 탭 → **Refresh All**.
5. SideStore → Sources → **+** → 아래 주소 추가 → Browse 탭에서 **이적시장 분석** → Install.
   ```
   https://raw.githubusercontent.com/sattosatto111/fc-market-download/main/source.json
   ```

### 알아둘 것
- 무료 Apple ID 서명은 7일마다 갱신해야 한다. WireGuard를 켜고 SideStore에서 Refresh All 하면 폰에서 바로 된다(PC 불필요).
- 무료 계정은 이렇게 넣은 앱을 3개까지만 둘 수 있다.
- 새 버전이 나오면 SideStore에 Update가 뜬다.
- 막히면 가장 흔한 원인 세 가지: 개발자 모드 꺼짐, iTunes 미설치(USB 인식 안 됨), WireGuard가 꺼져 있음.
