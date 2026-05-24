린매스업 트래커 PWA — 설치 안내
=====================================

[방법 A] GitHub Pages 무료 호스팅 (추천: 폰 어디서나 접속)
----------------------------------------------------------
1. github.com 가입/로그인
2. 우측 상단 + → New repository
   - Repository name: leanmass (아무 이름)
   - Public 선택 → Create repository
3. "uploading an existing file" 클릭
4. 이 폴더의 5개 파일 모두 드래그 업로드:
   index.html, manifest.json, service-worker.js, icon-192.png, icon-512.png
   → Commit changes
5. 상단 Settings → 좌측 Pages
   - Branch: main / (root) 선택 → Save
6. 1~2분 후 주소 생성: https://[아이디].github.io/leanmass/
7. 폰에서 그 주소 접속

[홈 화면에 앱으로 설치]
- iPhone(Safari): 공유 버튼 → "홈 화면에 추가"
- Android(Chrome): 우측 점3개 → "앱 설치" 또는 "홈 화면에 추가"
→ 아이콘 생성, 전체화면 실행, 오프라인 작동

[방법 B] 호스팅 없이 폰에서 바로 (간단, 단 오프라인 앱설치는 X)
----------------------------------------------------------
index.html을 폰으로 전송 후 브라우저로 열기.
* 단, file:// 로 열면 서비스워커(오프라인)는 작동 안 함.
  localStorage 저장은 정상 작동.

[중요 - 데이터 백업]
- 기록은 기기 1대에만 저장됨. 폰 변경/캐시삭제 시 소실.
- 목표 탭 → CSV 내보내기로 주기적 백업 권장.
