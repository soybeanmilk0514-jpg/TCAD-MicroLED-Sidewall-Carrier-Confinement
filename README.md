# TCAD MicroLED Sidewall Carrier Confinement

InGaN/GaN MicroLED의 측벽 결함에 의한 비방사 재결합을 분석하고, **Carbon 고저항 edge와 국부 AlGaN 측면 장벽**의 캐리어 구속 메커니즘을 비교하는 공동 프로젝트입니다.

**2026.09–현재 · 진행 중**  
학교 **CMP 프로그램**과 **공학및 지식실무 교과목**에서 동시에 진행하고 있습니다.  
**연구팀: 이택규 · 주수빈** / **주수빈 담당: 공통 baseline 검토 및 Project B — Localized AlGaN Lateral Heterobarrier**

**Summary:**  
An ongoing Sentaurus TCAD study of sidewall recombination in InGaN/GaN MicroLEDs, comparing carbon-induced high-resistivity edges with localized AlGaN lateral heterobarriers under a common baseline.

---

## Status at a Glance

| Item | Current status |
|---|---|
| 연구 단계 | Phase 0 — 공통 기준 모델 검증 |
| 주수빈 최신 실행 기록 · 2026.09.26 | `NtSide=0` 완료 / `NtSide=1e18` 실패 — 사용자 보고 기반 OBSERVED |
| 현재 우선 과제 | 실패 node의 실제 `*.err` / `*.out` 로그로 원인 식별 |
| 기존 미해결 항목 | SDevice2 → SVisual2 TDR 출력 파일 연결 |
| Project A / B | TCAD 구현·비교 설계 수립, 공통 baseline 동결 후 검증 예정 |
| 성능 결론 | IQE 개선 및 A/B 우열은 아직 검증되지 않음 |

실행 완료는 소자 물리 검증 완료를 의미하지 않습니다. 과거 SDevice2 정상 종료 기록과 오늘의 특정 split-run 실패 기록은 서로 다른 실행 맥락으로 보존했습니다.

## Team & My Contribution

| Member | Scope |
|---|---|
| **주수빈** | 공통 모델의 코드·실행 조건 검토, 계산 시간 및 split-run 상태 확인, **Project B의 국부 AlGaN 측면 장벽 설계**, 문헌 근거와 비교 방법 정리 |
| **이택규** | 공통 모델 구축·검증, **Project A의 Carbon-induced high-resistivity edge**, 공동 연구 저장소와 진행 기록 관리 |

개인 기여 근거: [주수빈 작업 기록](./CMP/members/JuSubin/TIMELINE.md) · [이택규 작업 기록](./CMP/members/LeeTaekGyu/TIMELINE.md) · [팀 타임라인](./CMP/TEAM_TIMELINE.md)

## Read the Project

| Page | Description |
|---|---|
| [Project Page](./index.md) | 목적·담당 업무·현재 상태 |
| [Detailed Navigation](./guide/00_navigation.md) | 전체 문서와 원본 코드 안내 |
| [Project Overview](./guide/01_project_overview.md) | 측벽 결함 문제와 공동 연구 범위 |
| [Common Baseline](./guide/02_common_baseline.md) | 문헌 기반 구조·물리 모델·검증 기준 |
| [Project B & Fair Comparison](./guide/03_project_b_and_comparison.md) | AlGaN 장벽 설계와 A/B 비교 계획 |
| [Progress & Limitations](./guide/04_progress_and_limitations.md) | 확인된 기록, 미해결 사항, 재현 범위 |
| [Source Code](./source/README.md) | 공개된 Sentaurus command·Tcl 위치 |
| [Recorded Results](./results/README.md) | 기존 calibration 기록과 진행 상태 구분 |
| [Source & Attribution](./report/README.md) | 원본 출처와 공동 작업 이력 보존 |
| [Research Dashboard](./docs/index.html) | 원본 형식의 대시보드 소스 |

## Repository Scope

[TaekGyu0801/GGYU](https://github.com/TaekGyu0801/GGYU)를 Fork하여 **원본 Git 이력과 `CMP/` 전체 자료**를 보존하고 개인 포트폴리오 안내를 추가했습니다. 2026-09-26 기준 공개 이슈 7개와 LIVE LOG 댓글 26개도 [읽기 전용 기록](./archive/upstream-issues.md)으로 보관했습니다.

이 저장소는 해당 시점의 포트폴리오 사본입니다. 공동 연구의 최신 기준은 [원본 연구 공간](https://github.com/TaekGyu0801/GGYU/tree/main/CMP)과 [공동 대시보드](https://taekgyu0801.github.io/GGYU/)이며, 이후 변경이 자동 동기화되지는 않습니다. 원본의 사전 준비 기록 날짜는 유지했습니다.

---

[← Back to Subin Joo's GitHub Portfolio](https://github.com/soybeanmilk0514-jpg)
