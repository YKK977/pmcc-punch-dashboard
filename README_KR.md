# Yanbu SRU PMCC Punch Dashboard - GitHub Pages 배포용

## 운영 방식
1. GitHub에 새 repository 생성: 예) `pmcc-punch-dashboard`
2. 이 폴더 안의 파일을 전부 업로드
   - `index.html`
   - `data/pmcc_source.xlsx`
3. Repository Settings > Pages
   - Source: `Deploy from a branch`
   - Branch: `main` / `/root`
   - Save
4. 생성된 Pages URL을 Notion에서 `/embed`로 삽입
5. 최신 원본 Excel이 생기면 `data/pmcc_source.xlsx`만 같은 이름으로 교체 업로드

## 중요
- Dashboard는 GitHub Pages에서 `data/pmcc_source.xlsx`를 자동으로 읽습니다.
- Notion에는 OneDrive 링크가 아니라 GitHub Pages URL을 Embed해야 합니다.
- 원본 Excel 열기/다운로드 버튼은 `data/pmcc_source.xlsx`를 가리킵니다.
