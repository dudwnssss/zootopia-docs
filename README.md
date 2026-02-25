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
| [UX_FLOW.md](./UX_FLOW.md) | 화면 흐름, 빌더/가이드 사용 시나리오, **기능 배치 기준(IA 원칙)** | 기획, 개발 |
| [ECONOMY.md](./ECONOMY.md) | 코인 경제 흐름, 밸런스 계산 | 기획, 개발 |
| [BALANCE.md](./BALANCE.md) | 게임 수치 히스토리 (가챠 확률, 비용 등) | 개발 |
| [TEACHER.md](./TEACHER.md) | 선생님 기능 요청 및 아이디어 | 기획 |

---

## 사용 방법

### 준엽/재평 (기획팀)
- 해당 파일에 직접 수정 or 레제한테 슬랙으로 말해도 됨
- 세계관/용어 → `WORLDBUILDING.md`
- 캐릭터 추가/수정 → `CHARACTERS.md`
- 미션 설계/아이디어 → `MISSION_DESIGN.md`
- 화면 흐름 변경 → `UX_FLOW.md`
- 코인/뽑기 밸런스 → `ECONOMY.md`
- 수치 히스토리 확인 → `BALANCE.md`
- 선생님 기능 요청/아이디어 → `TEACHER.md` ⭐

### 영준 (개발)
- 개발 전 해당 문서 확인
- 새 기능 요청 오면 레제가 슬랙으로 컨펌 요청함 → OK/수정/보류 결정
- 수치 변경은 `ECONOMY.md` → `BALANCE.md` → `game-config.ts` 순서로

### 레제 (AI)
- 기획 문서가 정답. 코드가 문서와 다르면 코드를 수정
- 텍스트/세계관/기존 기능 개선 → 바로 반영
- **새 기능 추가 → 영준 컨펌 먼저, 그 다음 개발**
- 문서 업데이트 요청 오면 GitHub에도 동기화

---

## 웹앱 링크
- 🌍 앱: https://web-eight-lime-11.vercel.app
- 🚀 온보딩: https://web-eight-lime-11.vercel.app/onboarding
- 📖 가이드: https://web-eight-lime-11.vercel.app/teacher/guide
