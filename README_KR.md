# Yanbu SRU PMCC Punch Dashboard v7

## 운영 방식
1. GitHub repo의 `data` 폴더에는 Excel 파일을 1개만 둡니다.
2. 파일명은 원본 그대로 유지합니다. 예: `(Consolidated) PMCC Punch List_20260624.xlsx`
3. 새 파일을 올릴 때는 기존 xlsx를 삭제하고 새 xlsx를 업로드합니다.
4. 대시보드는 GitHub API로 `data` 폴더의 xlsx 파일명을 확인한 뒤, 해당 파일을 읽어 자동 표시합니다.
5. 열람자는 `Download Source Excel` 버튼으로 현재 원본 Excel을 다운로드할 수 있습니다.

## 보안 메모
- GitHub Pages 공개 저장소(public repo)에 올리면 Dashboard와 Excel 원본은 링크를 아는 사람이 접근할 수 있습니다.
- 별도 토큰이나 비밀번호는 HTML에 저장하지 않습니다.
- 회사 내부 자료라면 GitHub 저장소 공개 범위를 반드시 확인하세요.
- private repo의 GitHub Pages는 조직/플랜 정책에 따라 동작 여부가 다를 수 있습니다.

## 계산 기준
- KPI는 `Overall Status` 시트의 `OVERALL` 블록 내 `Sub Total` 행만 사용합니다.
- PMCC별 막대/표는 각 PMCC 블록의 `Sub Total` 행을 사용합니다.
- PMCC-01, PMCC-02는 Completed로 고정 표시합니다.
