# IT·기술 영상 만들기

## 유튜브 채널

- 채널 URL: https://www.youtube.com/@코구리-k2o

## 제출 영상

- 주제: SQL JOIN 6가지 총정리 (INNER · LEFT · RIGHT · FULL OUTER · CROSS · SELF)
- 영상 URL: https://www.youtube.com/shorts/hKZWy33cLio

---

## 채널 소개

**코딩하는 너구리**는 수업에서 배운 백엔드·CS 개념을 1~2분짜리 세로 쇼츠로 정리하는 "개발 백과" 채널입니다.

| 카테고리 | 영상 | 길이 | 주소 |
|---|---|---|---|
| SQL | SQL JOIN 6가지 총정리 (제출 영상) | 1:57 | https://www.youtube.com/shorts/hKZWy33cLio |
| SQL | LEFT JOIN 했는데 회원이 사라졌다? WHERE vs ON | 1:40 | https://www.youtube.com/shorts/WYv_WygDKiU |

## 제출 영상 정보

- 형식: 세로 9:16 (1080×1920), 1분 57초
- 나레이션: Edge TTS 한국어 음성(ko-KR-InJoonNeural)
- 자막: 나레이션과 단어 단위로 맞춘 한국어 자막
- 화면: 같은 예시 데이터(회원 3명 · 주문 4건)로 조인마다 결과 표가 어떻게 바뀌는지 보여 줌
- 공개 상태: 공개, 로그인 없이 시청 가능

## 제작 과정

Claude Code와 함께 아래 순서로 만들었습니다.

1. **대본 먼저:** 주제를 정하면 장면 순서, 나레이션, 화면 구성, 예상 길이를 담은 대본을 먼저 받고 검토했습니다.
2. **내용 검토:** 대본을 확정하기 전에 예시 쿼리의 결과 행과 NULL을 하나씩 따져 보고, 틀린 설명을 고쳤습니다.
   - 예: MySQL에는 FULL OUTER JOIN이 없어 LEFT JOIN과 RIGHT JOIN을 합쳐야 합니다. 이때 `UNION`은 정당한 중복 행까지 지우므로, 화면 코드는 `UNION ALL` + `WHERE u.id IS NULL` 방식으로 바로잡았습니다.
3. **제작:** Edge TTS로 나레이션과 단어별 타이밍을 만들고, HyperFrames(HTML + GSAP)로 장면을 만든 뒤 자동 검사, 장면 캡처 확인, 렌더링을 거쳤습니다.
4. **확인과 수정:** 완성 영상을 직접 재생해 보고 목소리, 자막 줄바꿈 등을 고쳐 다시 렌더링했습니다.
5. **업로드:** YouTube Data API로 썸네일과 함께 비공개 업로드한 뒤, Studio에서 확인하고 공개로 전환했습니다. 영상은 카테고리별 재생목록(SQL)에 넣었습니다.
6. **학습 기록:** 영상마다 예상 면접 질문과 답변을 카테고리별 노트로 이어서 정리합니다.
