# Yanbu SRU PMCC Punch Dashboard v8

## 운영 방식
- GitHub에는 `index.html`만 올립니다.
- PMCC 원본 Excel은 GitHub에 올리지 않습니다.
- 각 사용자가 `Load Source Excel`로 회사 SharePoint/OneDrive에서 받은 원본 Excel을 한 번 선택합니다.
- 선택된 Excel은 해당 사용자의 브라우저 IndexedDB에 저장되어 다음 접속 시 자동 복원됩니다.
- `Download Loaded Excel`은 사용자가 로드한 원본 Excel을 다시 다운로드하는 버튼입니다.
- `Clear Local Data`는 현재 브라우저에 저장된 Excel을 삭제합니다.

## 보안
- GitHub Pages에 Excel 원본을 올리지 않습니다.
- 토큰/비밀번호/API key를 사용하지 않습니다.
- Excel은 각 사용자의 브라우저 로컬 저장소에만 보관됩니다.

## GitHub 업로드
기존 repo에서 `index.html`만 v8 파일로 교체하세요.
`data` 폴더와 Excel 파일은 삭제해도 됩니다.
