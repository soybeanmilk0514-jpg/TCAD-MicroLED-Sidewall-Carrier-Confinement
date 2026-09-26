# Common Baseline

이 문서는 [원본 COMMON_BASELINE](../CMP/COMMON_BASELINE.md)을 읽기 쉽게 요약합니다. 연구 파라미터를 변경하거나 새 실행 결과를 추가하지 않았습니다.

| 항목 | 기준 |
|---|---|
| Geometry | 2D Cartesian, 대표 mesa 폭 4 µm |
| MQW | In0.15Ga0.85N QW 4개 × 3 nm, GaN barrier 5개 × 22 nm |
| n-GaN | 4.0 µm, Nd=5e18 cm⁻³ |
| p-side | Al0.15Ga0.85N EBL 26 nm, p-GaN 120 nm |
| Sidewall | DmgL / Clean / DmgR 분할, 손상 두께 5 nm |
| Trap starting point | acceptor bulk trap, Ev+0.75 eV, Nt=1e18 cm⁻³, σn=σp=1e-15 cm² |
| Environment | 300 K, Cartesian, cylindrical OFF |
| Physics | Fermi, polarization, SRH/radiative/Auger, mobility 및 incomplete ionization |

JBD의 4 µm pixel pitch는 응용 규모의 참고입니다. 이 모델의 mesa 폭과 같은 실측 치수이거나 실제 상용 소자 복제라고 주장하지 않습니다. 수직 epitaxy, 측벽 손상 표현, 크기 효과의 근거는 각 문헌에서 구분하여 가져왔습니다. trap 값과 유효 도핑에는 모델링 가정·calibration 대상이 포함됩니다.

## Validation Sequence

1. 구조·영역·접촉·mesh·도핑을 확인.
2. Defect OFF의 정상 LED 동작을 검증.
3. Defect ON의 측벽 SRH 증가와 IQE 변화를 검증.
4. Nt, mesa 크기, mesh 및 2D 전류 정규화 민감도를 확인.
5. 공통 baseline을 동결한 후 A/B 구조만 변화.

Workbench 흐름: SDE → SDevice1(OFF) → SVisual1(I–V) → SDevice2(ON) → SVisual2(field maps).

[원본 참고자료 색인](../CMP/references/TCAD_REFERENCE_INDEX.md)
