# 트랜스제주 100마일 시뮬레이터

브라우저에서 하는 트랜스제주 100마일 트레일러닝 게임. 순위는 Firebase Firestore `records` 컬렉션에 쌓입니다.

## 파일
- `index.html` — 게임 전체
- `firebase-config.js` — Firebase 웹 앱 설정값 (여기만 수정)
- `firestore.rules` — Firestore 보안 규칙 (읽기 공개, 기록 추가만 허용, 수정·삭제 금지)

## 배포
1. Firebase 콘솔에서 프로젝트 생성 → Firestore Database 만들기(프로덕션 모드) → 규칙 탭에 `firestore.rules` 내용 붙여넣고 게시
2. 프로젝트 설정 → 내 앱 → 웹 앱의 `firebaseConfig` 값이 `firebase-config.js`에 들어 있음
3. GitHub 저장소에 세 파일을 올리고 Settings → Pages → Branch `main` / root 로 배포
