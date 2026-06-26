# PMCC Dashboard v9 - Notion + GitHub Pages + JSON

## 운영 방식
- 일반 URL: 대시보드만 표시
- 관리자 URL: `?admin=1` 붙이면 Excel Load / JSON Export 버튼 표시

## 업데이트 절차
1. `https://ykk977.github.io/pmcc-punch-dashboard/?admin=1` 접속
2. `Load Source Excel` 클릭 후 최신 원본 Excel 선택
3. 숫자 확인
4. `Export dashboard.json` 클릭
5. GitHub repo의 `data/dashboard.json` 파일을 이 파일로 교체
6. Notion 대시보드 자동 갱신

## 보안
- 원본 Excel은 GitHub에 업로드하지 않음
- GitHub에는 집계 JSON만 업로드
- Tag, Punch 상세, Comment 등 민감한 세부내용은 포함하지 않음


## v11 변경
- Last Updated 중복 표시 제거: 상단 우측 배지만 유지
- Dashboard 본문에는 Source File만 표시
