# Zootopia 기획 문서

> **이 파일들이 정답입니다. 코드는 이 문서를 따릅니다.**
> 문서를 수정하면 코드도 그에 맞게 수정됩니다.

---

## 문서 구조 한눈에 보기

```
┌─────────────────────────────────────────────────────┐
│                   WORLDBUILDING.md                   │
│        세계관 · 용어 · 등급 체계 (모든 문서의 기반)         │
└──────────┬──────────────┬──────────────┬────────────┘
           │              │              │
    ┌──────▼──────┐  ┌────▼──────┐  ┌───▼────────┐
    │CHARACTERS.md│  │MISSION_   │  │ ECONOMY.md │
    │캐릭터 40종  │◄─►│DESIGN.md  │  │ 코인 경제  │
    │등급·대사·관계│  │캐릭터×미션│  │ 흐름 설계  │
    └─────────────┘  └───────────┘  └─────┬──────┘
                                          │
                                    ┌─────▼──────┐
    ┌─────────────┐  ┌──────────┐   │ BALANCE.md │
    │  UX_FLOW.md │◄─┤TEACHER.md│   │ 수치 정답  │
    │ 화면흐름·IA │  │선생님기능│   │(숫자 변경시│
    │  배치 기준  │  │  명세    │   │  여기서만) │
    └─────────────┘  └──────────┘   └────────────┘
```

---

## 문서별 역할

| 문서 | 한 줄 요약 | 주로 보는 사람 |
|------|-----------|--------------|
| [WORLDBUILDING.md](./WORLDBUILDING.md) | 세계관·용어·등급 체계 — **모든 문서의 기반** | 전체 |
| [CHARACTERS.md](./CHARACTERS.md) | 캐릭터 40종 목록, 등급, 대사, 관계도 | 기획·개발 |
| [MISSION_DESIGN.md](./MISSION_DESIGN.md) | 캐릭터별 미션 매트릭스, 미션 설계 철학 | 기획 |
| [UX_FLOW.md](./UX_FLOW.md) | 화면 흐름 + 기능 배치 기준(IA 원칙) | 기획·개발 |
| [ECONOMY.md](./ECONOMY.md) | 코인 획득·소비 경로, 경제 흐름 원칙 | 기획·개발 |
| [BALANCE.md](./BALANCE.md) | **수치 정답** (가챠 확률, 비용, 스탯 등) | 개발 |
| [TEACHER.md](./TEACHER.md) | 선생님 기능 명세, GitHub Issue 안내 | 기획 |

---

## 추천 읽기 순서

처음 접하는 사람이라면 이 순서로 읽는 것을 권장:

```
1. WORLDBUILDING.md   — 세계관과 용어부터 파악
2. CHARACTERS.md      — 어떤 캐릭터들이 있는지
3. MISSION_DESIGN.md  — 캐릭터들이 어떤 미션을 내는지
4. ECONOMY.md         — 코인이 어떻게 흐르는지
5. UX_FLOW.md         — 화면이 어떻게 구성되는지
6. TEACHER.md         — 선생님 기능 상세
7. BALANCE.md         — 필요할 때만 (수치 확인)
```

---

## 문서 간 의존 관계

- **용어**는 `WORLDBUILDING.md`가 정의. 다른 문서에서 쓰는 단어(빌더, 가이드, 스카우트 등)는 모두 여기서 확인.
- **수치**는 `BALANCE.md`가 정답. `ECONOMY.md`는 원칙, `BALANCE.md`는 숫자.
- **캐릭터**와 **미션**은 `CHARACTERS.md`와 `MISSION_DESIGN.md`가 함께 읽혀야 완성.
- **화면 경로** (`/teacher/notices` 등)는 `UX_FLOW.md`에 정의. `TEACHER.md`에서 이를 참조.

---

## 사용 방법

### 준엽 / 재평 (기획)
슬랙에서 레제한테 말해도 됨. 직접 수정도 OK.
- 세계관·용어 → `WORLDBUILDING.md`
- 캐릭터 추가·수정 → `CHARACTERS.md`
- 미션 설계 → `MISSION_DESIGN.md`
- 화면 흐름 변경 → `UX_FLOW.md`
- 코인·뽑기 밸런스 → `ECONOMY.md` → `BALANCE.md`
- 선생님 기능 요청 → `TEACHER.md` 또는 [GitHub Issues](https://github.com/dudwnssss/zootopia-docs/issues)

### 영준 (개발)
- 기능 개발 전 해당 문서 확인
- 수치 변경: `ECONOMY.md` 원칙 확인 → `BALANCE.md` 수정 → `game-config.ts` 반영
- 새 기능: 레제가 슬랙으로 컨펌 요청 → OK/수정/보류 결정

### 레제 (AI)
- 문서가 정답. 코드가 다르면 코드를 수정.
- 새 기능 추가 → 영준 컨펌 먼저.
- 문서 수정 시 GitHub에 push.

---

## 웹앱 링크
- 🌍 앱: https://web-eight-lime-11.vercel.app
- 📖 가이드: https://web-eight-lime-11.vercel.app/teacher/guide
