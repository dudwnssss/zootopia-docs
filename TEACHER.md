# 가이드(선생님) 기능 명세

> 선생님(가이드) 입장에서 사용하는 기능들의 명세.
> 기능 요청/아이디어는 → **[GitHub Issues](https://github.com/dudwnssss/zootopia-docs/issues)** 에 올려줘.

---

## 현재 구현된 기능

| 기능 | 경로 | 설명 |
|------|------|------|
| 퀘스트 생성/관리 | `/teacher/missions` | 미션 만들고 빌더에게 배정 |
| 빌더 목록 / 코인 관리 | `/teacher/classes` | 반 빌더 목록, 코인 수동 지급/차감 |
| 자리배치도 | `/teacher/tools` | 드래그앤드롭 자리배치, Supabase 연동 |
| QR코드 초대 | `/teacher/qrcodes` | 빌더 초대용 QR |
| 가이드 가이드 | `/teacher/guide` | 기능 설명 온보딩 |
| 알림장 | `/teacher/notices` | 알림장 작성/발송, 반별 목록, 빌더 홈에서 열람 |

---

## 기능 요청 방법

**슬랙에 말로 해도 됨** — 레제가 GitHub Issue로 정리해줄게.

```
"레제야, [기능 이름] 기능 필요해 — [간단한 설명]"
```

또는 직접 Issue 열기:
→ https://github.com/dudwnssss/zootopia-docs/issues/new

---

## Issue 라벨 설명

| 라벨 | 의미 |
|------|------|
| `status: 컨펌대기` | 영준 컨펌 기다리는 중 |
| `status: 진행중` | 개발 진행 중 |
| `status: 완료` | 개발 완료 |
| `status: 보류` | 일단 보류 |
| `cat: 선생님기능` | 가이드 관련 기능 |
| `cat: 학생기능` | 빌더 관련 기능 |
| `cat: UI/UX` | 화면/디자인 개선 |
| `cat: 인프라` | DB, 아키텍처 관련 |
| `priority: high` | 빠르게 |
| `priority: mid` | 보통 |
| `priority: low` | 나중에 |

---

## 현장 인사이트

- **일방소통 선호**: 선생님들은 개인 연락 없이 공지만 하고 싶어함. 전화는 교실 내선만.
  → 알림장/공지 기능이 핵심
- **배포 전략** (2026-02-25 준엽): 기본 학급관리+안내 시스템 + 개인농장 꾸미기 + 학급 마을 꾸미기 세트 완성 후 배포
