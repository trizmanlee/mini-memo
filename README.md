# 미니 PC 요청함

폰이 손에 없을 때 PC 브라우저에서 미니(개인 비서)에게 할 일이나 메모를 남기는 아주 작은 페이지입니다.

- 주소: https://trizmanlee.github.io/mini-memo/
- 요청은 Google Forms로 접수되어 미니가 몇 분 안에 확인합니다.
- 비밀코드와 보낸 기록은 브라우저의 `localStorage`에만 저장됩니다. 서버나 저장소에는 아무것도 남지 않습니다.
- 연락처·이메일 주소 같은 개인정보는 코드에 들어 있지 않습니다.

## 구성

| 항목 | 내용 |
| --- | --- |
| `index.html` | 페이지 전체 (HTML + CSS + JS, 외부 의존성 없음) |
| 전송 | Google Form `formResponse`로 `fetch(..., { mode: 'no-cors' })` POST |
| 단축키 | `Enter` 전송, `Shift`+`Enter` 줄바꿈 |

GitHub Pages(브랜치 `main`, 경로 `/`)로 배포됩니다. 별도 빌드 과정은 없습니다.
