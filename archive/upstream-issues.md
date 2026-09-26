# Upstream issue archive

Snapshot: 2026-09-26 UTC. Source: https://github.com/TaekGyu0801/GGYU/issues

공개 이슈 7개와 LIVE LOG 댓글 26개를 읽기 전용으로 보관합니다. 작성자·날짜·원문 링크를 유지합니다. 이슈의 제안·관찰·미해결 상태는 원문 기준이며 검증된 성능으로 해석하지 않습니다. 최신 공동 작업은 원본 저장소를 확인하세요.

## #7 LIVE LOG — 이택규 · 주수빈 · ChatGPT · Claude 연구 진행 기록

Author: TaekGyu0801 · Created: 2026-09-21T08:38:14Z · Updated: 2026-09-22T06:38:58Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/7

# CMP Live Research Log

이 Issue는 여러 노트북 / 여러 GPT 계정 / Claude에서 발생한 **중요한 연구 진행과 문제를 시간순으로 모으는 공용 이벤트 로그**다.

## 기록 대상
- 새 blocker 발생
- 오류 원인 확인
- 코드 수정
- 시뮬레이션 성공/실패
- 중요한 연구 판단
- 다음 작업 확정
- 다른 AI에게 넘길 내용

## 기록하지 않는 것
- 단순 잡담
- 아직 채택되지 않은 사소한 아이디어
- 중복된 상태 보고

## Comment format

```text
[날짜/시간]
작업자: 이택규 / 주수빈
AI: ChatGPT / Claude
구분: PROGRESS / BLOCKER / FIX / RESULT / DECISION / HANDOFF

요약:
...

근거:
- 실제 로그/스크린샷/코드/결과

변경:
- 파일/파라미터/코드

상태:
- OBSERVED / CONFIRMED / PROPOSED / UNRESOLVED / REJECTED

다음:
...
```

각 AI는 의미 있는 작업이 끝나면 이 Issue에 comment를 추가하고,
필요 시 CURRENT_STATUS / ERROR_LOG / member TIMELINE / .ai-sync도 갱신한다.


### Comment 5757727616

Author: TaekGyu0801 · Created: 2026-09-21T08:41:16Z · Updated: 2026-09-21T08:41:16Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5757727616

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA

요약:
새 채팅에서 작업자 이름(이택규/주수빈)을 입력하면 GitHub 최신 상태를 읽고 현재 진행·현재 blocker·개인 최신 기록·다음 작업을 첫 답변에서 브리핑하는 규칙을 추가함.

변경:
- CMP/SESSION_START_PROTOCOL.md 생성
- CMP/AGENTS.md 갱신
- CMP/CHAT_TO_GITHUB_PROTOCOL.md 갱신
- Issue #7 공용 LIVE LOG 연결

상태:
CONFIRMED

다음:
각 참여 GPT/Claude가 GitHub 저장소 접근 권한과 프로젝트 시작 지침을 가지고 이 프로토콜을 실행하도록 구성.



---

### Comment 5758274926

Author: TaekGyu0801 · Created: 2026-09-21T09:26:58Z · Updated: 2026-09-21T09:26:58Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758274926

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION

요약:
주수빈도 CMP 프로젝트 안에서 새 채팅 첫 메시지로 "주수빈"이라고 입력해 작업자를 식별하고, GitHub 최신 상태 브리핑 + 자동 기록 흐름을 사용하기로 함.

상태:
CONFIRMED

조건:
주수빈 계정에서도 GGYU 저장소 읽기/쓰기 접근 권한이 필요함.



---

### Comment 5758356486

Author: TaekGyu0801 · Created: 2026-09-21T09:33:23Z · Updated: 2026-09-21T09:33:23Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758356486

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: PROGRESS / INFRA

요약:
이택규가 주수빈 GitHub 계정을 GGYU collaborator로 초대했다고 보고함.

상태:
OBSERVED (사용자 보고 기준)

다음:
주수빈이 초대를 수락한 뒤 GitHub username 기준 collaborator permission 확인 → 주수빈 GPT/Claude에서 GGYU 읽기/쓰기 테스트.



---

### Comment 5758366165

Author: TaekGyu0801 · Created: 2026-09-21T09:34:10Z · Updated: 2026-09-21T09:34:10Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758366165

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: PROGRESS / INFRA

요약:
주수빈 GitHub 계정 `soybeanmilk0514-jpg`의 GGYU collaborator 권한을 확인함.

결과:
permission = write

상태:
CONFIRMED

다음:
주수빈 ChatGPT/Claude 계정에서 GitHub 연결 후 GGYU 읽기/쓰기 테스트.



---

### Comment 5758501755

Author: TaekGyu0801 · Created: 2026-09-21T09:45:22Z · Updated: 2026-09-21T09:45:22Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758501755

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA

요약:
이택규 GPT / 주수빈 GPT / Claude가 같은 CMP 프로젝트에서 사용할 공통 협업 규칙을 확정함.

추가:
- CMP/AI_COLLAB_RULES.md

핵심:
- 이름으로 작업자 고정
- 세션 시작 시 GitHub 최신 상태 브리핑
- 의미 있는 작업 자동 기록
- 개인/팀 기록 분리
- 코드 수정 전 최신 원본 확인
- Common Baseline 보호
- 동시 작업 충돌 방지
- .ai-sync 기반 AI 인수인계

상태:
CONFIRMED



---

### Comment 5758521179

Author: TaekGyu0801 · Created: 2026-09-21T09:46:58Z · Updated: 2026-09-21T09:46:58Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758521179

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA

요약:
새 채팅에서 "이택규" 또는 "주수빈"으로 시작하면 첫 답변에 다음을 항상 포함하도록 규칙을 업데이트함.

- 현재까지 진행 상황
- 가장 마지막으로 한 작업
- 현재 blocker
- 다음 작업
- CMP 대시보드 링크

대시보드:
https://taekgyu0801.github.io/GGYU/

상태:
CONFIRMED


---

### Comment 5758554485

Author: TaekGyu0801 · Created: 2026-09-21T09:49:47Z · Updated: 2026-09-21T09:49:47Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758554485

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA
상태: CONFIRMED

요약:
CMP AI Shared Memory Protocol v2를 구축함. 이택규 GPT / 주수빈 GPT / Claude가 세션 시작 시 최신 GitHub 상태를 읽고, 의미 있는 연구 결과를 작업 중 자동으로 GitHub에 기록하도록 최상위 규칙을 통합함.

변경:
- CMP/AI_SHARED_MEMORY_PROTOCOL.md 생성
- CMP/.ai-sync/SYNC_STATE.json 생성
- CMP/AGENTS.md를 master protocol 진입점으로 정리
- CMP/AUTO_LOG_POLICY.md의 Issue #undefined 오류를 #7로 수정
- CMP/.ai-sync/README.md에 Protocol v2 연결
- CMP/TEAM_TIMELINE.md 기록

핵심 동작:
READ-first → 작업 → 의미 있는 결과 WRITE → Issue #7 append → 필요 시 RELAY handoff

주의:
AI는 백그라운드에서 서로의 채팅을 읽는 것이 아니라 GitHub에 실제로 기록된 내용을 통해 동기화함.



---

### Comment 5758582576

Author: TaekGyu0801 · Created: 2026-09-21T09:52:02Z · Updated: 2026-09-21T09:52:02Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758582576

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA
상태: CONFIRMED

요약:
Claude가 GGYU/CMP의 최신 상태를 읽고 현재 연구 지점에서 코드 작성·디버깅·검증을 이어서 수행하도록 전용 GitHub 작업 프롬프트를 추가함.

변경:
- CMP/prompts/CLAUDE_GITHUB_WORK_PROMPT.md 생성

핵심:
READ GitHub first → understand current blocker/code → minimal code change → validate → WRITE meaningful result back to GitHub.



---

### Comment 5758660568

Author: TaekGyu0801 · Created: 2026-09-21T09:58:52Z · Updated: 2026-09-21T09:58:52Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758660568

[2026-09-21]
작업자: 이택규
AI: ChatGPT
구분: PROGRESS / REFERENCE
상태: CONFIRMED

요약:
사용자가 제공한 Sentaurus T-2022.03 공식 User Guide(SDevice/SDE/SMesh/SVisual)와 예제 자료를 검토해 CMP reference index에 등록함.

핵심 확인:
- Solar-cell 공식 example에서 SDevice File block의 Workbench macro pattern 확인:
  grid=@tdr@ / current=@plot@ / output=@log@ / plot=@tdrdat@ / parameter=@parameter@
- 현재 SDevice2→SVisual2 blocker에서는 macro를 추측으로 변경하기보다 pp9_des.cmd의 실제 preprocessed File block 확인이 우선.

변경:
- CMP/references/TCAD_REFERENCE_INDEX.md
- CMP/references/TCAD_REFERENCE_MANIFEST.md
- CMP/AI_SHARED_MEMORY_PROTOCOL.md
- CMP/TEAM_TIMELINE.md

주의:
Synopsys User Guide의 proprietary notice 때문에 원본 PDF/전체 example source는 public repository에 복제하지 않음.



---

### Comment 5758784007

Author: TaekGyu0801 · Created: 2026-09-21T10:09:31Z · Updated: 2026-09-21T10:09:31Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758784007

[2026-09-21 19:02]
작업자: 이택규
AI: ChatGPT
구분: PROGRESS / TEAM SYNC
상태: OBSERVED

요약:
공유 프로젝트의 주수빈 채팅에서 확인된 병렬 연구 진행을 CMP GitHub에 동기화함.

주수빈 진행:
- 메인 SDevice 및 앞서 검토된 관련 코드를 최종 수정했다고 사용자 보고
- Project A/B 공통 Common Baseline으로 적합한지 장시간 simulation 전 최종 검토 단계
- 우선 NtSide=0, NtSide=1e18 두 조건을 먼저 실행할 계획
- 사용자 보고 기준 약 3일/run 소요 가능

검증 경계:
- 주수빈 측 최신 전체 코드 원문과 새 simulation 결과는 현재 GitHub에서 직접 검증되지 않음
- 따라서 코드 정확성/실행 성공은 아직 CONFIRMED 아님

변경:
- CMP/members/JuSubin/TIMELINE.md
- CMP/TEAM_TIMELINE.md
- CMP/CURRENT_STATUS.md
- CMP/NEXT_ACTIONS.md
- CMP/.ai-sync/LIVE_STATE.md
- CMP/.ai-sync/LIVE_STATE.json

다음:
주수빈 측 최신 전체 코드 동기화 → 정적/논리 검토 → NtSide=0 / 1e18 실행 → 결과/로그 기록.


---

### Comment 5758978873

Author: TaekGyu0801 · Created: 2026-09-21T10:25:24Z · Updated: 2026-09-21T10:25:24Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5758978873

[2026-09-21 19:05]
작업자: 이택규
AI: ChatGPT
구분: DECISION / INFRA
상태: CONFIRMED

요약:
CMP 프로젝트 안에서 수행하는 의미 있는 연구 작업은 작업자가 이택규/주수빈 누구든 별도 "저장해" 요청 없이 GitHub에 자동 기록하도록 범위를 재확정함.

포함:
- 코드 수정
- 오류 발생/해결
- simulation 결과
- baseline/설계 판단
- blocker 변경
- 다음 작업 변경
- 인수인계

제외:
- 단순 잡담
- 일반 개념 질문
- 아직 연구에 반영하지 않은 사소한 아이디어

경계:
AI가 볼 수 없는 다른 비공개 채팅을 실시간으로 직접 읽는다고 가정하지 않음. 각 채팅의 AI가 GitHub에 기록하면 다음 AI가 이어받을 수 있음.

변경:
- CMP/AI_SHARED_MEMORY_PROTOCOL.md
- CMP/AI_COLLAB_RULES.md
- CMP/TEAM_TIMELINE.md


---

### Comment 5770898802

Author: soybeanmilk0514-jpg · Created: 2026-09-22T03:44:16Z · Updated: 2026-09-22T03:44:16Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5770898802

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: BLOCKER / DIAGNOSTIC
상태: OBSERVED / UNRESOLVED

요약:
NtSide=0, 1e18 split 실행 과정에서 사용자가 SWB에서 SDE보다 SDevice가 먼저 실행되는 것처럼 보인다고 보고함.

판단:
- NtSide가 SDevice에만 쓰이고 기존 SDE geometry/mesh output이 유효하다면, SWB가 upstream SDE를 재사용하고 SDevice split부터 실행하는 것은 정상일 수 있음.
- SDE가 한 번도 성공적으로 실행되지 않은 신규/clean 상태인데 SDevice가 먼저 시작된다면 dependency 또는 File/Grid 연결 점검 필요.

다음:
pp*_des.cmd의 File { Grid=... }와 실제 SDE mesh TDR 존재 여부를 확인한 뒤 정상 재사용인지 연결 오류인지 판정.


---

### Comment 5770952468

Author: soybeanmilk0514-jpg · Created: 2026-09-22T03:52:03Z · Updated: 2026-09-22T03:52:03Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5770952468

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: FIX / DIAGNOSTIC
상태: CONFIRMED

요약:
Node 6 Explorer의 pp6_des.cmd를 확인해 SDE→SDevice 연결이 정상임을 확인함.

근거:
- Grid = "n1_msh.tdr"
- Node 6 output에 n6_des.tdr / n6_des.plt / n6_des.log 존재

판단:
SDevice Node 6는 SDE Node 1의 mesh를 정상 재사용 중이다. NtSide가 SDE geometry를 변경하지 않는 현재 split에서는 SDE가 다시 실행되지 않고 SDevice부터 실행되는 것이 정상 동작으로 판단됨.


---

### Comment 5770973393

Author: soybeanmilk0514-jpg · Created: 2026-09-22T03:55:01Z · Updated: 2026-09-22T03:55:01Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5770973393

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: BLOCKER / RUNTIME DIAGNOSTIC
상태: OBSERVED

요약:
전날 밤부터 18시간 이상 실행 중인 Node 6 SDevice output을 확인함. 현재 화면상 계산은 멈춘 것이 아니라 BE stepping을 계속 수행 중임.

근거:
- 직전 step: |Rhs| < 1.0000E-03 로 수렴 완료
- 누적 wallclock: Assembly 598.77 s, Solve 2928.83 s, Total 3563.68 s (~59 min/step)
- 다음 step: 약 0.0766738 -> 0.0776738, Stepsize=1.0000E-03

판단:
현재 증거는 fatal/hang보다 매우 큰 per-step 계산비용을 가리킴. 18시간 미완료 자체는 이 step cost와 양립함.

다음:
pp6_des.cmd Solve block의 최종 target 및 InitialStep/MinStep/MaxStep/Increment/ramp 설정을 확인해 총 step 수와 예상 runtime을 산정. Common Baseline physics는 이 진단 때문에 변경하지 않음.


---

### Comment 5771026401

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:02:40Z · Updated: 2026-09-22T04:02:40Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771026401

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: BLOCKER / DIAGNOSIS
상태: CONFIRMED

요약:
Node 6 장시간 run의 직접적인 numerical 원인을 pp6_des.cmd와 n6_des.out로 확인함.

근거:
- Transient: InitialStep=1e-5, MinStep=1e-9, MaxStep=1e-3, Increment=1.2
- Goal: anode Voltage=5.0 V
- log pseudo-time 0.0766738에서 anode ≈0.3834 V, 5×0.0766738≈0.38337 V와 일치
- 따라서 MaxStep=1e-3은 최대 약 5 mV/bias step에 해당
- 현재 지점에서 5 V까지 최소 약 923~924 accepted steps가 남음

영향:
최근 관찰된 약 3564 s/step을 단순 외삽하면 약 38일 규모가 될 수 있음(실제 step cost는 bias에 따라 변동).

다음:
pp6_des.cmd 자체가 아니라 원본 SDevice deck의 numerical stepping을 검토. Common Baseline physics는 변경하지 않음.


---

### Comment 5771045053

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:05:23Z · Updated: 2026-09-22T04:05:23Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771045053

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: DIAGNOSIS REFINEMENT
상태: OBSERVED / UNRESOLVED

추가 정보:
사용자가 최종 수정 전 거의 같은 코드가 약 3일 내 완료된 이력이 있다고 보고함.

정정:
현재 MaxStep=1e-3은 많은 step 수를 설명하지만, 이번 run이 과거보다 느려진 '새 원인'으로 단정할 수 없음. 이전 run도 같은 step-control이었다면 per-step solve cost 증가 또는 rejected/cutback 증가가 핵심 후보.

우선 비교:
1) old/new Transient step settings
2) mesh 규모
3) Physics/Traps 적용 범위
4) Math solver 설정
5) .out의 failed/retry/cutback 및 Newton iteration 수

주의:
최근 3564 s 한 step에서 나온 ~38일 값은 거친 선형 외삽일 뿐 실제 ETA로 취급하지 않음.


---

### Comment 5771092412

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:11:57Z · Updated: 2026-09-22T04:11:57Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771092412

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: RESULT / RUNTIME COMPARISON
상태: OBSERVED

과거 약 3일 내 완료된 run의 초기 .out 로그를 확인함.

관찰:
- anode=0 V 초기 coupled solve
- Assembly ≈350.52 s
- Solve ≈232.46 s
- Total ≈585.81 s
- 약 50 Newton iterations 후 |RHS| < 1e-3 수렴

주의:
현재 run의 ~0.38 V step(total ~3563.68 s)과 bias가 달라 직접 비교는 아직 불가.

다음:
과거 run의 anode 0.3~0.4 V 구간에서 동일 형식 로그를 찾아 Total time/iteration/retry를 비교.


---

### Comment 5771105776

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:13:46Z · Updated: 2026-09-22T04:13:46Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771105776

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: RESULT / RUNTIME COMPARISON
상태: OBSERVED

과거 약 3일 내 완료된 run의 .out에서 0.30 V 부근 step 비용을 확인함.

관찰:
- anode ≈0.3034 V: Total 172.57 s (Assembly 35.80 s, Solve 136.34 s)
- anode ≈0.3084 V: Total 123.94 s (Assembly 42.71 s, Solve 78.79 s)
- 두 step 모두 Newton iteration 0~4 후 |RHS|<1e-3 수렴

현재 run 비교:
- anode ≈0.3834 V에서 Total ≈3563.68 s/step 관찰

판단:
동일 bias는 아니지만 현재 run의 per-step 계산비용이 과거 run보다 크게 증가한 정황이 강함. 과거 0.38 V 부근 로그를 추가 확인해 최종 정량 비교 필요.


---

### Comment 5771125739

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:16:17Z · Updated: 2026-09-22T04:16:17Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771125739

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: RESULT / RUNTIME ROOT-CAUSE NARROWING
상태: CONFIRMED

동일 bias 직접 비교:
- old run, anode ≈0.3834 V: Assembly 64.84 s, Solve 108.74 s, Total 177.47 s
- current run, anode ≈0.3834 V: Assembly 598.77 s, Solve 2928.83 s, Total 3563.68 s

결론:
현재 accepted step wallclock이 old 대비 약 20.1배 증가. 이번 slowdown은 MaxStep/step count 자체보다 per-step solve cost 증가가 핵심.

다음:
old/current의 mesh/grid/unknown statistics, Physics/Traps 적용 범위, Math/solver 설정, Newton/linear iteration 비용을 우선 비교.


---

### Comment 5771152799

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:19:44Z · Updated: 2026-09-22T04:19:44Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771152799

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: CORRECTION / RUNTIME DIAGNOSIS
상태: CONFIRMED CORRECTION + UNRESOLVED CAUSE

중요 정정:
앞서 0.303~0.3834 V에서 Total 123~177 s인 로그를 과거 3일 run으로 해석했으나, 새 스크린샷의 경로와 사용자 설명을 통해 해당 로그 역시 현재 Node 6의 동일 n6_des.out 초기 구간임을 확인함.

현재 run 내부 관찰:
- 초기 0.0756738→0.0766738, anode ≈0.3834 V: Total 177.47 s
- 더 뒤쪽 화면에서 anode ≈0.3834 V 직후: Total 3563.68 s

따라서 기존 'old vs current 20.1x slowdown' 결론은 무효.
새 핵심 질문은 같은 run 내부에서 동일 pseudo-time/voltage ramp가 여러 Transient/Solve stage에서 반복되는지 여부임.

다음:
pp6_des.cmd에서 Transient( 검색 횟수 확인, n6_des.out에서 3563.68 및 0.0766738의 반복 위치를 확인해 느린 stage를 식별.


---

### Comment 5771164958

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:21:32Z · Updated: 2026-09-22T04:21:32Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771164958

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: CORRECTION / RUNTIME COMPARISON
상태: CONFIRMED

사용자 재확인:
직전 0.3834 V / Total 177.47 s 스크린샷은 현재 run이 아니라 예전에 약 3일 만에 완료된 노드의 n6_des.out임.

따라서 동일-bias 비교는 유효:
- old ≈0.3834 V: Assembly 64.84 s, Solve 108.74 s, Total 177.47 s
- current ≈0.3834 V: Assembly 598.77 s, Solve 2928.83 s, Total 3563.68 s
- current ≈20.1× slower per accepted step

앞서 기록한 'same current run repeated stage' 해석은 철회.
다음은 old/current의 Math/solver, Physics/Traps 적용 범위, mesh/grid/unknown statistics 비교.


---

### Comment 5771211697

Author: soybeanmilk0514-jpg · Created: 2026-09-22T04:28:07Z · Updated: 2026-09-22T04:28:07Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5771211697

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: RESULT / OLD DECK CAPTURE
상태: OBSERVED

사용자가 과거 약 3일 내 완료된 node의 full pp6_des.cmd를 제공함.

핵심:
- old deck의 모든 DmgL/R trap Conc = 0 → NtSide=0 케이스
- Transient: InitialStep=1e-5, MinStep=1e-9, MaxStep=1e-3, Increment=1.2, Goal anode=5 V
- current slow run에서 이미 확인한 step-control과 동일
- Math: 4 threads, Digits=5, ErrRef=1e4, RHSMin=1e-3, BE, ExtendedPrecision(80), Blocked + ILS(22), gmres(100), tolrel=1e-10, ilut(1e-8,-1)

다음:
현재 slow Node 6의 trap Conc가 0인지 1e18인지 먼저 확인. current도 0일 때만 old/current runtime을 직접 비교하고, 그 다음 Math/Physics/mesh diff 진행.


---

### Comment 5772096384

Author: soybeanmilk0514-jpg · Created: 2026-09-22T06:23:25Z · Updated: 2026-09-22T06:23:25Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5772096384

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: PRESENTATION / CES2027
상태: PROPOSED

요약:
다음 주 월요일 15분 CES2027 선발 발표 준비를 시작함. 지난 1주차의 일반 배경 반복은 줄이고, literature-grounded Common Baseline 근거 → 구조/TCAD validation → 동일 baseline에서 Project A/B를 공정 비교하는 구현 전략을 핵심 스토리라인으로 설정.

발표 핵심 source 역할:
- JBD: application/product scale
- Kou 2019: vertical blue InGaN/GaN epitaxy backbone
- Wu 2023: localized ~5 nm sidewall damage physics
- Chen 2024: small (~4×4 µm-class) microLED sidewall-effect relevance

주의:
현재 미완료 SDevice 장시간 run은 confirmed result처럼 발표하지 않고 structural validation과 electrical/optical validation을 구분함.

변경:
- CMP/CES2027_PRESENTATION_PLAN.md 생성
- JuSubin/TIMELINE.md, TEAM_TIMELINE.md 업데이트

다음:
슬라이드별 문구, 그림, 논문 citation 및 발표 대본을 구체화.


---

### Comment 5772139162

Author: soybeanmilk0514-jpg · Created: 2026-09-22T06:28:08Z · Updated: 2026-09-22T06:28:08Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5772139162

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: PRESENTATION / SOURCE REVIEW
상태: OBSERVED

요약:
사용자가 CES2027 1주차 발표 PPT(7 slides)를 제공함. 1주차는 JBD target, microLED scaling-sidewall loss, 연구주제 진화, Carbon vs AlGaN 전략, CES에서 확인할 product/manufacturing relevance를 중심으로 구성되어 있었음.

2주차 발표 방향 반영:
- scaling/sidewall 일반 배경 반복 최소화
- Week 1 -> Week 2 progress bridge 1장
- baseline 문헌 provenance/수치 근거/TCAD 구조 검증 중심
- A/B는 기존 concept 반복보다 실제 TCAD 구현 및 fair-comparison design을 추가
- CES relevance는 후반부에 유지

주의:
원본 PPT에는 개인 식별 정보가 있어 공개 GitHub에 파일 자체는 업로드하지 않고, 발표 기획 내용만 기록함.

변경:
- CMP/CES2027_PRESENTATION_PLAN.md 업데이트


---

### Comment 5772241509

Author: soybeanmilk0514-jpg · Created: 2026-09-22T06:38:58Z · Updated: 2026-09-22T06:38:58Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5772241509

[2026-09-22]
작업자: 주수빈
AI: ChatGPT
구분: DESIGN / PRESENTATION
상태: PROPOSED

요약:
교수진의 1차 발표 피드백에 답하기 위해 Project A/B의 구체적인 TCAD 구현 계획을 정의함.

Project A:
- 고정 5 nm sidewall damage 안쪽에 edge-localized high-resistivity GaN:C guard/current-blocking region
- 우선 upper n-GaN near-MQW에 배치
- carbon deep-acceptor/compensation model을 calibration parameter로 사용
- 목표: current/carrier를 중앙으로 재분배하고 sidewall SRH 감소 확인

Project B:
- 고정 damage 안쪽 active-region lateral path에 localized AlGaN heterobarrier
- x_Al / lateral width DOE
- 목표: lateral Ec/Ev barrier, carrier confinement, sidewall SRH 감소 확인

공통:
- same-current 비교
- SRH / Radiative / Auger / IQE / Vf / current crowding / carrier-current maps
- exact process dimensions remain PROPOSED, not frozen

변경:
- CMP/PROJECT_AB_TCAD_IMPLEMENTATION_PLAN.md 생성
- JuSubin/TIMELINE.md 업데이트


---

### Comment 5843505191

Author: soybeanmilk0514-jpg · Created: 2026-09-26T05:24:06Z · Updated: 2026-09-26T05:24:06Z

Source: https://github.com/TaekGyu0801/GGYU/issues/7#issuecomment-5843505191

[2026-09-26]
작업자: 주수빈
AI: ChatGPT
구분: RESULT / BLOCKER
상태: OBSERVED / UNRESOLVED

요약:
학교에서 이전 Common Baseline split run을 확인한 결과 NtSide=0은 정상 완료, NtSide=1e18은 failed 상태로 확인됨.

근거:
- 사용자가 Sentaurus Workbench 상태 화면 직접 제공

현재 판단:
- 실패 원인은 아직 미확인.
- 0 조건 성공만으로 1e18 실패를 trap physics 자체 문제라고 단정하지 않음.

다음:
- failed 1e18 SDevice node의 *.err 전체
- *.out 마지막 50~100줄
- 가능하면 node 번호 / pp*_des.cmd
를 확인해 최초 fatal/convergence error를 식별한 뒤 최소 수정.

보호 조건:
- 원인 확인 전 Common Baseline Nt/Et/sigma/5 nm damage width/epitaxy 변경 금지.


---

## #6 Phase 5 — Final report / presentation

Author: TaekGyu0801 · Created: 2026-09-21T05:41:58Z · Updated: 2026-09-21T05:41:58Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/6

## Goal
근거 수준과 simulation validation을 분리해 최종 보고서/발표를 구성한다.

- [ ] source-role table
- [ ] Common Baseline validation figures
- [ ] Project A mechanism/results
- [ ] Project B mechanism/results
- [ ] A/B comparison
- [ ] limitations
- [ ] reproducibility appendix



---

## #5 Phase 4 — Project A vs B fair comparison

Author: TaekGyu0801 · Created: 2026-09-21T05:41:56Z · Updated: 2026-09-21T05:41:56Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/5

## Goal
동일한 baseline과 동일한 defect 조건에서 두 confinement mechanism을 비교한다.

- [ ] same baseline confirmation
- [ ] same current-density comparison
- [ ] I-V penalty comparison
- [ ] sidewall SRH suppression
- [ ] radiative recombination
- [ ] IQE
- [ ] mechanism interpretation
- [ ] limitations



---

## #4 Phase 3 — Project B: Localized AlGaN Lateral Heterobarrier

Author: TaekGyu0801 · Created: 2026-09-21T05:41:54Z · Updated: 2026-09-21T05:41:54Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/4

## Goal
동일한 Common Baseline에서 localized AlGaN energetic confinement을 검증한다.

Expected chain:
AlGaN lateral barrier → lateral diffusion ↓ → sidewall carrier density ↓ → fixed sidewall SRH ↓

- [ ] AlGaN source/parameter review
- [ ] barrier geometry
- [ ] Al fraction / width sensitivity
- [ ] lateral band profile
- [ ] carrier distribution
- [ ] SRH comparison
- [ ] IQE at same current density



---

## #3 Phase 2 — Project A: Carbon High-R Edge

Author: TaekGyu0801 · Created: 2026-09-21T05:41:53Z · Updated: 2026-09-21T05:41:53Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/3

## Goal
동일한 Common Baseline에서 Carbon-induced resistive confinement을 검증한다.

Expected chain:
Carbon → compensation → edge resistance ↑ → edge current/carrier access ↓ → fixed sidewall defect interaction ↓ → SRH ↓

- [ ] Carbon model/source review
- [ ] Carbon placement/edge width 정의
- [ ] Carbon concentration sweep
- [ ] I-V 영향 확인
- [ ] sidewall carrier-access map
- [ ] SRH comparison
- [ ] IQE at same current density



---

## #2 Phase 1 — Freeze Common Baseline Final

Author: TaekGyu0801 · Created: 2026-09-21T05:41:51Z · Updated: 2026-09-21T05:41:51Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/2

## Goal
Phase 0 validation을 통과한 Common Baseline을 동결한다.

- [ ] Geometry final
- [ ] Physics final
- [ ] Defect OFF/ON comparison final
- [ ] Current normalization rule documented
- [ ] IQE extraction documented
- [ ] Baseline code snapshot preserved
- [ ] Project A/B 공통 조건 문서화

Common Baseline을 freeze하기 전 Project A/B의 성능 결론을 확정하지 않는다.



---

## #1 Phase 0 — Common Baseline validation

Author: TaekGyu0801 · Created: 2026-09-21T05:41:50Z · Updated: 2026-09-21T05:41:50Z · State: open

Source: https://github.com/TaekGyu0801/GGYU/issues/1

## Goal
Common Baseline v1이 의도한 geometry와 sidewall-defect physics를 재현하는지 검증한다.

## Required checks
- [x] DmgL / Clean / DmgR region partition 존재 확인
- [x] 4 QWs + 5 barriers 존재 확인
- [x] p/n doping scale 시각 확인
- [x] SVisual1 forward I-V Tcl 오류 해결
- [ ] SDevice2 TDR output filename/linkage 해결
- [ ] Defect OFF 정상 LED 동작 확인
- [ ] Defect ON sidewall recombination 증가 확인
- [ ] Radiative/IQE degradation 확인
- [ ] Nt sensitivity
- [ ] mesa-size sensitivity
- [ ] mesh convergence

## Source of truth
- CMP/COMMON_BASELINE.md
- CMP/CURRENT_STATUS.md
- CMP/ERROR_LOG.md


