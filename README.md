# 매매 프로젝트 (안드로이드 설치용)

## 폴더 구성
- index.html — 앱 본체
- manifest.webmanifest — 앱 이름·아이콘·전체화면 설정
- sw.js — 오프라인에서도 열리게 하는 캐시
- icon-192.png, icon-512.png, icon-maskable-512.png — 앱 아이콘

## GitHub Pages에 올리기
1. github.com 로그인 → 오른쪽 위 + → New repository
2. 이름 예: maemae → Public 선택 → Create repository
3. "uploading an existing file" 클릭 → 이 폴더의 파일 7개 전부 끌어다 놓기 → Commit changes
4. 저장소 Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save
5. 1~2분 뒤 https://아이디.github.io/maemae/ 주소가 생김

## 폰에 설치
1. 안드로이드 크롬에서 위 주소 열기
2. ⋮ 메뉴 → "앱 설치" (또는 "홈 화면에 추가" → 설치)
3. 홈 화면 아이콘으로 실행 — 전체 화면, 오프라인에서도 동작

## 데이터
- 데이터는 폰(브라우저 저장소)에만 저장됨. 서버로 아무것도 안 보냄.
- 관리 탭 → 데이터 백업 → "백업 저장"으로 JSON 파일을 주기적으로 저장해 두기.
- 폰 교체·앱 삭제·크롬 사이트 데이터 삭제 전에는 꼭 백업.
- 새 폰에서는 앱 설치 후 "백업 불러오기"로 복구.

## 앱을 고쳤을 때
- index.html을 바꿔 올린 뒤 sw.js 맨 위 VERSION 값을 올리기 (예: maemae-v1 → maemae-v2)
- 폰에서 앱을 한 번 열었다 닫으면 새 버전이 반영됨.

## 참고
- 저장소를 Public으로 해도 데이터는 올라가지 않음 (코드만 공개).
- 세금 계산은 간이 추정치. 실제 신고는 세무사 확인.
