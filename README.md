# 움직이는 전선 v3

6·25 전쟁의 전선 이동과 주요 사건을 순차적으로 학습하는 Next.js 웹앱입니다.

## 구조
- `app/` : 화면과 전역 스타일
- `components/` : 인트로, 지도, 연대기, 사건 패널, 전체 애니메이션
- `data/events.ts` : 사건·날짜·기간·전선·이동경로·관련자료 데이터
- `public/maps/` : 업로드한 한반도 산지 지도
- `public/video/` : 업로드한 인트로 영상

## 실행
```bash
npm install
npm run dev
```

## 배포
GitHub 저장소에 프로젝트 전체를 올린 뒤 Vercel에서 저장소를 Import하면 됩니다. Framework Preset은 Next.js로 자동 감지됩니다.

## 주의
지도 위 전선 및 이동 경로는 현재 학습용 개략 좌표입니다. 실제 작전 지도와 날짜별 전선을 더 정밀하게 반영하려면 `data/events.ts`의 SVG 경로 좌표를 검증·보정하세요.
