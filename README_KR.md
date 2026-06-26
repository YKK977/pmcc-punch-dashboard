# Yanbu SRU PMCC Punch Dashboard

## GitHub Pages 업로드 방법

Repository 루트에 아래 파일/폴더를 그대로 업로드합니다.

```text
index.html
data/status.json
data/pmcc_source.xlsx
```

GitHub Pages URL 예:

```text
https://ykk977.github.io/pmcc-punch-dashboard/
```

Notion에서는 `/embed` 입력 후 위 URL을 붙여넣으면 됩니다.

## 주간 업데이트 방법

현재 대시보드는 `data/status.json`을 읽습니다.

- 원본 Excel 다운로드 버튼은 `data/pmcc_source.xlsx`를 가리킵니다.
- 최신 원본을 공유하려면 `data/pmcc_source.xlsx`를 최신 파일로 교체합니다.
- 수치 업데이트는 `data/status.json`만 교체하면 됩니다.

## PMCC Master

PMCC-01 및 PMCC-02는 Completed로 고정되어 있습니다.
PMCC-03~PMCC-14는 향후 데이터가 들어오면 `status.json`에서 Total/Remaining 등을 채우면 자동 표시됩니다.
