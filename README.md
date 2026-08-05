# reports

`report.redevpartners.net` 로 서비스되는 리포트 아카이브 (GitHub Pages).

## 구조

```
index.html        리포트 목록 페이지 (manifest.json 을 읽어 렌더)
manifest.json     게시 목록. 배포 스크립트가 갱신한다.
reports/          실제 리포트 HTML 파일
CNAME             커스텀 도메인
.nojekyll         Jekyll 처리 비활성화
```

## manifest.json 형식

```json
[
  { "title": "데일리 다이제스트 (오전)", "date": "2026-08-05",
    "path": "reports/2026-08-05-digest-am.html" }
]
```

날짜 내림차순으로 index.html 이 알아서 정렬한다.

## 주의

이 저장소는 **공개(public)** 다. 여기에 커밋되는 순간 누구나 볼 수 있고 검색엔진에
색인될 수 있다. 게시 대상만 선별해서 넣는다.
