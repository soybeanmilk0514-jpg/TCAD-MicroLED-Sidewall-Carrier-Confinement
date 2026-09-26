# Progress & Limitations

Snapshot: **2026-09-26**.

## Latest Observation

[오늘의 상태 기록](../CMP/CURRENT_STATUS.md)에 따르면 주수빈의 NtSide=0 run은 완료, NtSide=1e18 run은 failed입니다. 사용자 화면 보고 기반 OBSERVED이며 실패 원인은 UNRESOLVED입니다. 실제 err 및 out 로그 확인 전 trap physics, syntax, convergence 또는 자원 문제 중 하나로 단정하지 않습니다.

## Previously Recorded Checks

2D 구조 및 DmgL/Clean/DmgR 분할, 4 QW/5 barrier, p/n 도핑 범위 시각 확인, SVisual1 Tcl 수정 후 실행 및 별도 SDevice2 solver 정상 종료가 원본에 기록되어 있습니다. SVisual2의 n9_des.tdr 로딩 문제는 별도 미해결 기록입니다. 서로 다른 날짜와 run의 기록을 단일 성공 결과로 합치지 않습니다.

## What Remains

Defect OFF/ON 물리 검증, 실패 node 진단, TDR 연결 확인, IQE 추출, Nt·크기·mesh 민감도, 공통 모델 동결 및 A/B 비교가 남아 있습니다.

## Reproducibility

공개 저장소에는 현재 SDevice2 command와 SVisual Tcl, P2 calibration deck·추출 Tcl·CSV, P3 재현 메모가 있습니다. 최신 전체 SDE/SDevice1 프로젝트, 모든 TDR/PLT/실행 로그 또는 완성된 A/B 결과가 공개되어 있지는 않습니다. 이번 포트폴리오 정리에서 Sentaurus를 새로 실행하지 않았습니다.

원본의 2026-08-27 P2/P3 기록은 사전 준비 checkpoint로 보존했습니다. 공식 프로젝트 기간은 사용자 제공 정보에 따라 2026.09–현재로 표시합니다. Synopsys 원문 매뉴얼·전체 라이선스 예제·비공개 서버 백업은 추가 공개하지 않습니다.
