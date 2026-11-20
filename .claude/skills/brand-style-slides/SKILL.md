---
name: "brand-style-slides"
description: "PPT·슬라이드·발표자료를 만들 때 사용자가 'Stripe 느낌으로', 'Apple 스타일로'처럼 브랜드 디자인을 고르거나 '디자인 목록 보여줘'라고 하면 사용. VoltAgent 디자인 시스템을 가져와 적용한다."
---

# 브랜드 스타일 슬라이드

VoltAgent의 awesome-design-md(MIT 라이선스)에 있는 브랜드별 DESIGN.md를 가져와, 그 색·글꼴·여백·분위기로 발표자료를 만든다.

## 1. 디자인 가져오기

```bash
git clone --depth=1 -q https://github.com/VoltAgent/awesome-design-md.git /tmp/awesome-design-md 2>/dev/null || true
ls /tmp/awesome-design-md/design-md
```

브랜드 파일 위치: `/tmp/awesome-design-md/design-md/<브랜드>/DESIGN.md`

주요 브랜드: apple, stripe, linear.app, ibm, notion, vercel, tesla, spacex, nvidia, samsung이 없으면 비슷한 계열 추천, airbnb, nike, spotify, figma, mastercard, bmw, ferrari, lamborghini, claude, sap, oracle, uber, wise, revolut 등 70여 개.

사용자가 브랜드를 정하지 않았거나 '목록 보여줘'라고 하면, 폴더 목록을 보여주되 용도별로 3~5개를 추천한다.
- 사내 보고·공공기관 보고: ibm, stripe, linear.app, sap, notion
- 기술·혁신 발표: nvidia, spacex, vercel, tesla
- 고급스러운 제안서: apple, bmw, ferrari

## 2. DESIGN.md 읽고 슬라이드 규칙으로 옮기기

DESIGN.md 전체를 읽은 뒤 아래만 뽑아 쓴다.
- colors: 바탕(canvas), 본문색(ink), 강조색(primary), 보조색 2~3개
- typography: 제목·본문 크기 비율, 굵기, 자간 성향
- 분위기: 여백 정도, 모서리 둥글기, 그림자 사용 여부, 그라데이션 여부

웹 화면용 값이므로 슬라이드에 맞게 바꾼다.
- 크기는 픽셀 그대로 쓰지 않고 비율만 따른다(16:9 기준 제목 28~40pt, 본문 14~18pt).
- 전용 글꼴(Sohne, SF Pro 등)은 쓸 수 없으므로 한글은 Pretendard 또는 맑은 고딕, 영문은 비슷한 산세리프로 바꾼다. 원본이 가는 굵기(300)여도 한글 가독성을 위해 제목은 600 이상으로 한다.
- 강조색은 슬라이드당 1~2곳에만 쓴다.

## 3. 만들기

- 형식을 지정하지 않으면 Slides 아티팩트로 만든다(PPT·PDF로 내려받기 가능). 사용자가 .pptx 파일을 명시하면 pptx 스킬로 만든다.
- 첫 슬라이드에 들어가기 전에, 고른 브랜드와 뽑은 핵심 규칙(색 3개, 글꼴, 분위기)을 한두 줄로 알려준다.

## 지켜야 할 것

- 디자인 분위기만 빌린다. 해당 회사의 로고·회사명·제품 이미지·슬로건은 넣지 않는다. 그 회사 자료처럼 보이게 만들지 않는다.
- 사내 보고서는 개조식 문장, 현황→문제→개선방안→기대효과 흐름을 기본으로 한다.
- 표·숫자가 많은 장표는 브랜드 스타일보다 가독성을 우선한다.