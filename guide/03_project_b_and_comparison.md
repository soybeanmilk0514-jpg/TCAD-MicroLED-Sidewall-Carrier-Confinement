# Project B & Fair Comparison

## 주수빈 담당 — Localized AlGaN Lateral Heterobarrier

MQW의 측면 캐리어 경로 안쪽에 국부 AlGaN 영역을 두어 band offset에 의한 캐리어 구속을 연구합니다. 목표는 손상 영역으로 이동하는 캐리어와 비방사 SRH 재결합을 줄이는 것입니다. 이는 **설계 가설**이며 IQE 향상을 확인한 결과가 아닙니다.

[원본 구현 계획](../CMP/PROJECT_AB_TCAD_IMPLEMENTATION_PLAN.md)에 제시된 후보 범위는 Al 조성 0.05 / 0.10 / 0.15 / 0.20 / 0.30, 장벽 폭 0.02 / 0.05 / 0.10 / 0.20 µm입니다. 동결된 최종값이나 실행 완료 sweep이 아닙니다.

## Project A — 이택규 담당

Carbon-induced high-resistivity edge는 보상에 의한 고저항 영역으로 측벽 방향 전류를 억제하는 안입니다. AlGaN의 band-offset 장벽과 작동 메커니즘을 구분합니다.

## Comparison Plan

| 고정 기준 | 비교 지표 |
|---|---|
| 동일 common baseline 및 측벽 손상 파라미터 | IQE와 SRH / radiative / Auger 재결합 |
| 동일 전류 밀도 | 동작 전압 Vf 및 carrier/current 분포 |
| 동일 integration 영역·정규화 | 측벽 재결합과 current crowding |
| mesh convergence 기준 | lateral Ec/Ev 및 구조별 물리적 해석 |

Baseline ON, A, B를 같은 전류 밀도에서 비교합니다. baseline의 Nt·Et·capture cross section·손상 두께를 구조별로 바꾸어 얻은 결과를 구조 개선 효과로 해석하지 않습니다. IQE와 EQE도 구분하며 광추출 효율 개선을 추정하지 않습니다.
