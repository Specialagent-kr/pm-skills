---
name: prioritization-frameworks
description: "9가지 우선순위 지정 프레임워크에 대한 참고 가이드입니다. 공식, 사용 시점 가이드 및 템플릿을 제공합니다. Opportunity Score, ICE, RICE, Kano, MoSCoW 등을 다룹니다. 우선순위 지정 방법을 선택하거나, 프레임워크를 비교하거나, 공식 정의가 필요할 때 사용하세요. 트리거: 우선순위 프레임워크, 어떤 프레임워크, ICE, RICE, opportunity score, Kano, MoSCoW, 우선순위 정하는 법."
---

# 우선순위 지정 프레임워크 참고 가이드

현재 상황에 맞는 적절한 우선순위 지정 프레임워크를 선택하고 적용하는 데 도움이 되는 참고 가이드입니다.

### 핵심 원칙

고객이 솔루션을 설계하게 하지 마십시오. 기능이 아니라 **문제(기회)**의 우선순위를 정하십시오.

### Opportunity Score (Dan Olsen, *The Lean Product Playbook*)

고객 문제를 우선순위화하는 데 권장되는 프레임워크입니다.

각 니즈에 대해 고객을 대상으로 **중요도(Importance)**와 **만족도(Satisfaction)**를 조사합니다 (0-1 범위로 정규화).

세 가지 관련 공식:

- **현재 가치(Current value)** = 중요도 × 만족도
- **기회 점수(Opportunity Score)** = 중요도 × (1 − 만족도)
- **창출된 고객 가치(Customer value created)** = 중요도 × (S2 − S1), 여기서 S1은 개선 전 만족도, S2는 개선 후 만족도입니다.

중요도는 높고 만족도는 낮은 항목이 가장 높은 기회 점수를 가지며, 이는 가장 좋은 기회를 의미합니다. 중요도 vs 만족도 차트에 표시하면 좌상단 사분면이 가장 공략하기 좋은 지점입니다. 이는 솔루션이 아닌 고객 문제의 우선순위를 정합니다.

### ICE 프레임워크

이니셔티브와 아이디어의 우선순위를 정하는 데 유용합니다. 가치뿐만 아니라 리스크와 경제적 요인도 고려합니다.

- **I** (Impact, 영향력) = 기회 점수 × 영향을 받는 고객 수
- **C** (Confidence, 자신감) = 우리의 확신 정도 (1-10). 리스크를 반영합니다.
- **E** (Ease, 용이성) = 구현이 얼마나 쉬운가? (1-10). 경제적 요인을 반영합니다.

**점수** = I × C × E. 점수가 높을수록 먼저 추진합니다.

### RICE 프레임워크

ICE의 영향력을 두 개의 별도 요인으로 나눕니다. 더 세분화된 관리가 필요한 대규모 팀에 유용합니다.

- **R** (Reach, 도달 범위) = 영향을 받는 고객 수
- **I** (Impact, 영향력) = 기회 점수 (고객당 가치)
- **C** (Confidence, 자신감) = 우리의 확신 정도 (0-100%)
- **E** (Effort, 노력) = 구현에 필요한 노력 (인월, person-months)

**점수** = (R × I × C) / E

### 9가지 프레임워크 개요

| 프레임워크 | 적합한 용도 | 주요 인사이트 |
|-----------|----------|-------------|
| 아이젠하워 매트릭스 | 개인 작업 | 긴급성 vs 중요성 — 개별 PM의 작업 관리에 적합 |
| 영향력 vs 노력 | 작업/이니셔티브 | 간단한 2×2 — 신속한 선별에 유용하나 전략적 결정에는 부족함 |
| 리스크 vs 보상 | 이니셔티브 | 영향력 vs 노력과 비슷하나 불확실성을 고려함 |
| **Opportunity Score** | 고객 문제 | **권장.** 중요도 × (1 − 만족도). 0–1로 정규화. |
| 카노(Kano) 모델 | 기대치 이해 | 반드시 있어야 함, 성능, 매력적, 무관심, 역행. 우선순위보다는 특성 이해용. |
| 가중치 의사결정 매트릭스 | 다요소 결정 | 기준에 가중치를 할당하고 각 옵션에 점수 부여. 이해관계자 합의에 유용. |
| **ICE** | 아이디어/이니셔티브 | 영향력 × 자신감 × 용이성. 빠른 우선순위 지정에 권장. |
| **RICE** | 대규모 아이디어 | (도달 범위 × 영향력 × 자신감) / 노력. ICE에 도달 범위를 추가. |
| MoSCoW | 요구사항 | Must/Should/Could/Won't. 주의: 프로젝트 관리 기반의 방식임. |

### 템플릿

- [Opportunity Score 소개 (PDF)](https://drive.google.com/file/d/1ENbYPmk1i1AKO7UnfyTuULL5GucTVufW/view)
- [중요도 vs 만족도 템플릿 — Dan Olsen (Google Slides)](https://docs.google.com/presentation/d/1jg-LuF_3QHsf6f1nE1f98i4C0aulnRNMOO1jftgti8M/edit#slide=id.g796641d975_0_3)
- [ICE 템플릿 (Google Sheets)](https://docs.google.com/spreadsheets/d/1LUfnsPolhZgm7X2oij-7EUe0CJT-Dwr-/edit?usp=share_link&ouid=111307342557889008106&rtpof=true&sd=true)
- [RICE 템플릿 (Google Sheets)](https://docs.google.com/spreadsheets/d/1S-6QpyOz5MCrV7B67LUWdZkAzn38Eahv/edit?usp=sharing&ouid=111307342557889008106&rtpof=true&sd=true)

---

### 더 읽어보기

- [The Product Management Frameworks Compendium + Templates](https://www.productcompass.pm/p/the-product-frameworks-compendium)
- [Kano Model: How to Delight Your Customers Without Becoming a Feature Factory](https://www.productcompass.pm/p/kano-model-how-to-delight-your-customers)
- [Continuous Product Discovery Masterclass (CPDM)](https://www.productcompass.pm/p/cpdm) (동영상 강의)
