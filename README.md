# LUMIVELIX 공식 홈페이지

[공식 홈페이지 미리보기 · PC / 모바일](https://ai-so20.github.io/Lumivelix-/)

루미벨릭스 AI 건강 링 공식 홈페이지의 정적 웹사이트 소스입니다.

## 구성

- `index.html`: GitHub Pages의 시작 페이지
- `.nojekyll`: 정적 파일을 그대로 게시하는 설정
- `dist/index.html`: 페이지와 메뉴·색상 선택·FAQ·안내 모달 동작
- `dist/assets/`: 제품 이미지와 스타일시트
- `dist/assets/fonts/`: Pretendard 가변 폰트와 OFL 라이선스
- `vercel.json`: 정적 배포 설정 (`dist` 출력 디렉터리)

## 로컬 확인

```sh
python3 -m http.server 8080 --directory dist
```

브라우저에서 http://localhost:8080 을 엽니다.

## Vercel 연결

이 저장소를 가져오고 프로젝트 루트를 저장소 루트로 선택합니다. Framework Preset은 Other, Output Directory는 `dist`를 사용합니다. 별도 빌드 명령이나 환경 변수는 필요하지 않습니다. Vercel 배포는 아직 진행하지 않았습니다.

## 검증 범위

- 320·390·430px 너비의 브라우저 화면에서 가로 넘침 확인
- 제품 이미지 및 로컬 폰트 로딩 확인
- 모바일 메뉴 열기·닫기와 앱 섹션 이동 확인
- 색상 선택, 기능 안내 모달, FAQ 확인

실제 iOS/Android 기기 검증은 별도로 필요합니다. 앱 화면은 이미지이므로 내부 글씨는 홈페이지 폰트 설정으로 바뀌지 않으며, 모바일에서는 원본 크게 보기로 확인할 수 있습니다.

이미지를 자르거나 해상도를 낮추지 않고 원본 파일을 포함했습니다. 홈페이지 폰트는 기존 Pretendard를 유지했습니다.
