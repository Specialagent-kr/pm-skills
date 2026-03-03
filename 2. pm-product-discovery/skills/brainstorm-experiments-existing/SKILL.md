---
name: brainstorm-experiments-existing
description: "기존 제품의 가설을 검증하기 위한 실험을 설계합니다. 프로토타입, A/B 테스트, 스파이크 및 기타 저비용 검증 방법을 제안합니다. 검증할 가설이 있거나, 전체 구현 전에 실험 아이디어가 필요하거나, 기능 아이디어를 저렴하게 테스트하고 싶을 때 사용하세요. 트리거: 실험 설계, 가설 테스트, 아이디어 검증, 프로토타입 테스트, A/B 테스트 아이디어."
---

# 실험 설계 (기존 제품)

전체 구현에 착수하기 전에 제품 가설을 테스트하기 위한 저비용 실험을 설계합니다.

### 맥락

당신은 **$ARGUMENTS**를 위한 실험을 설계하는 제품 팀을 돕고 있습니다. 팀은 기능 아이디어와 검증이 필요한 가설을 가지고 있습니다.

사용자가 파일(PRD, 가설 목록, 디자인 등)을 제공하면 먼저 읽으십시오.

### 지침

사용자가 아이디어와 가설을 설명할 것입니다. 다음 단계에 따라 작업을 진행하십시오:

1. **아이디어 및 가설 명확화**: 팀이 무엇을 만들고자 하는지, 그리고 무엇을 검증해야 하는지 확인하십시오.

2. **각 가설에 대한 실험 제안**. 다음과 같은 방법들을 고려하십시오:
   - 프로토타입을 이용한 첫 클릭 테스트(First-click testing) 또는 과업 완료 테스트
   - 기능 스텁(Feature stubs) 또는 페이크 도어(Fake door) 테스트
   - 기술적 스파이크(Technical spikes)
   - 운영 환경에서의 A/B 테스트 (리스크 완화 포함)
   - 오즈의 마법사(Wizard of Oz) 접근 방식
   - 설문 조사 기반 검증 (의견이 아닌 행동 중심)

3. **준수해야 할 핵심 원칙**:
   - 사용자의 의견이 아닌 실제 **행동**을 측정하십시오.
   - 책임감 있게 테스트하십시오 — 사용자나 비즈니스를 위험에 빠뜨리지 마십시오.
   - 운영 환경 테스트(예: A/B 테스트)의 경우 리스크 완화 전략을 설명하십시오.
   - 최소한의 노력으로 최대한의 검증된 학습(Validated Learning)을 목표로 하십시오.

4. **각 실험에 대해 다음 내용을 명시**:
   - **가설**: 우리가 믿고 있는 것은 무엇인가?
   - **실험**: 그것을 검증하기 위해 정확히 무엇을 할 것인가?
   - **지표**: 무엇을 측정할 것인가?
   - **성공 임계값**: 우리의 가설이 맞을 경우 예상되는 수치

단계별로 생각하십시오. 실험 내용을 명확한 표나 구조화된 형식으로 제시하십시오. 내용이 방대하면 마크다운으로 저장하십시오.

---

### 더 읽어보기

- [Testing Product Ideas: The Ultimate Validation Experiments Library](https://www.productcompass.pm/p/the-ultimate-experiments-library)
- [Assumption Prioritization Canvas: How to Identify And Test The Right Assumptions](https://www.productcompass.pm/p/assumption-prioritization-canvas)
- [What Is Product Discovery? The Ultimate Guide Step-by-Step](https://www.productcompass.pm/p/what-exactly-is-product-discovery)
- [Continuous Product Discovery Masterclass (CPDM)](https://www.productcompass.pm/p/cpdm) (동영상 강의)
