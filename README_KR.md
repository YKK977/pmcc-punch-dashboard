# Yanbu SRU PMCC Punch Dashboard v13

## 기준
- 데이터 기준 시트: `Summary by GS PIC`
- 원본 Excel은 GitHub에 올리지 않습니다.
- `data/dashboard.json`만 교체하면 Notion 대시보드가 갱신됩니다.

## 운영
1. 관리자 URL 접속: `...?admin=1`
2. `Load Source Excel` 클릭 후 최신 PMCC Excel 선택
3. `Export dashboard.json` 클릭
4. GitHub 저장소의 `data/dashboard.json`만 덮어쓰기

## v13 변경
- Process Engineering Status에 Total/Remaining/Close Requested/Closed/Clarification 추가
- Process Engineering Status 하단에 PMCC별 Process 상세 테이블 추가
- Summary Table의 PR 컬럼 삭제
- `Overall Status` 기준 로직 제거, `Summary by GS PIC` 기준 유지
