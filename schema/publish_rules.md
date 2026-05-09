# Publish Rules

1. `/write <topic>`은 항상 draft 상태의 topic page를 생성한다.
2. 생성 위치는 `topics/<topic-slug>/index.md`이다.
3. `metadata.json`의 status가 `reviewed`인 문서만 published 상태로 바꿀 수 있다.
4. GitHub repository 참고 자료에는 URL, star 수, star 수집 날짜를 남긴다.
5. `ONTOLOGY_HUB_AUTO_PUSH=1`인 환경에서는 `/write <topic>`이 생성한 topic folder를 자동 commit/push한다.
6. 자동 publish 상태 변경은 하지 않는다. 사람이 검토한 뒤 `/reviewed <document_id_or_slug>`와 `/publish <document_id_or_slug>`를 실행한다.
