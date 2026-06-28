# PMCC Dashboard v12

## 기준 변경
- 원본 Excel의 `Summary by GS PIC` 시트 기준으로 dashboard.json을 생성합니다.
- `Overall Status` 시트는 더 이상 사용하지 않습니다.

## 업로드 구조
GitHub Pages 저장소에는 아래 두 개만 유지합니다.

```text
index.html
data/dashboard.json
```

## 업데이트 방법
1. 대시보드 URL 뒤에 `?admin=1` 추가
2. `Load Source Excel` 클릭
3. 최신 `(Consolidated) PMCC Punch List_YYYYMMDD.xlsx` 선택
4. 화면 숫자 확인
5. `Export dashboard.json` 클릭
6. GitHub의 `data/dashboard.json`만 덮어쓰기

원본 Excel은 GitHub에 올리지 않습니다.
