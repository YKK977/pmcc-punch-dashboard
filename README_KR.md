# Yanbu SRU PMCC Punch Dashboard v5

## 운영 방식

GitHub repo의 `data` 폴더에 PMCC 원본 Excel 파일을 올리면 됩니다.

예시:

```text
data/
  (Consolidated) PMCC Punch List_20260620.xlsx
  (Consolidated) PMCC Punch List_20260624.xlsx
```

대시보드는 `data` 폴더 안의 `.xlsx/.xlsm/.xls` 파일을 GitHub API로 조회한 뒤, 파일명에 포함된 `YYYYMMDD`가 가장 최신인 파일을 자동 로드합니다.

## 파일명 규칙

파일명은 고정할 필요 없습니다. 다만 최신 파일 판단을 위해 `20260624` 같은 8자리 날짜가 들어가면 가장 안정적입니다.

## 버튼 설명

- `Reload Source Excel`: GitHub `data` 폴더에서 최신 Excel 다시 로드
- `Preview Local Excel`: 내 PC의 Excel을 임시 미리보기. GitHub에는 저장되지 않음
- `Download Source Excel`: 현재 대시보드가 읽은 원본 Excel 다운로드

## 계산 기준

- KPI는 `Overall Status` 시트의 `OVERALL` 블록 아래 `Sub Total` 행만 사용합니다.
- PMCC별 Chart는 각 PMCC 블록의 `Sub Total` 행을 사용합니다.
- PMCC-01/02는 Completed로 고정 표시합니다.
- PMCC-01~14까지 Master 목록에 반영했습니다.
