# Zootopia 기획 문서

> 이 레포는 Zootopia 앱의 기획/설계 스펙 문서 모음입니다.
> **이 파일들이 정답입니다. 코드는 이 문서를 따릅니다.**

---

## 문서 목록

| 파일 | 내용 | 주로 보는 사람 |
|------|------|--------------|
| [WORLDBUILDING.md](./WORLDBUILDING.md) | 세계관, 용어, 빌더/마을 등급 | 전체 |
| [CHARACTERS.md](./CHARACTERS.md) | 캐릭터 40종 목록, 등급, 대사 | 기획, 개발 |
| [MISSION_DESIGN.md](./MISSION_DESIGN.md) | 미션 설계, 캐릭터×미션 매트릭스 | 기획 |
| [UX_FLOW.md](./UX_FLOW.md) | 화면 흐름, 빌더/가이드 사용 시나리오 | 기획, 개발 |
| [ECONOMY.md](./ECONOMY.md) | 코인 경제 흐름, 밸런스 계산 | 기획, 개발 |

---

## 사용 방법

### 준엽/재평 (기획팀)
- 기획 변경 → 해당 파일에 직접 댓글 or 영준한테 전달
- 세계관/용어 → `WORLDBUILDING.md`
- 캐릭터 추가/수정 → `CHARACTERS.md`
- 미션 설계 → `MISSION_DESIGN.md`
- 화면 흐름 아이디어 → `UX_FLOW.md`
- 수치/밸런스 → `ECONOMY.md`

### 영준 (개발)
- 개발 전 해당 문서 확인
- 문서 변경사항 있으면 레제한테 "문서 보고 반영해줘" 요청
- 수치 변경은 `ECONOMY.md` → `BALANCE.md` → `game-config.ts` 순서로

### 레제 (AI)
- 기획 문서가 정답. 코드가 문서와 다르면 코드를 수정
- 문서 업데이트 요청 오면 GitHub에도 동기화

---

## 웹앱 링크
- 🌍 앱: https://web-eight-lime-11.vercel.app
- 🚀 온보딩: https://web-eight-lime-11.vercel.app/onboarding
- 📖 가이드: https://web-eight-lime-11.vercel.app/teacher/guide
