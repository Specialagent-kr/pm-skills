# PM 스킬 저장소: 더 나은 제품 의사결정을 위한 AI 운영 체제

> 65개 이상의 PM 스킬을 통해 제품 발견(Discovery)부터 전략, 실행, 출시 및 성장까지 제품 관리의 전 과정을 지원합니다.

이 프로젝트는 Pawel Huryn의 [pm-skills](https://github.com/phuryn/pm-skills)를 포크하여 한국어로 번역한 저장소입니다.

이 저장소는 AI툴 활용시 제품 관리자의 업무를 더 효과적으로 도울 수 있도록 설계된 전문 스킬 모음입니다.

## 왜 PM 스킬 저장소인가요?

일반적인 AI는 텍스트를 제공하지만, PM 스킬 저장소는 **구조**를 제공합니다.

각 스킬은 검증된 PM 프레임워크(발견, 가설 매핑, 우선순위 지정, 전략 등)를 토대로 설계되었으며, 단계별 워크플로우를 안내합니다. Teresa Torres, Marty Cagan, Alberto Savoia와 같은 전문가들의 방법론이 단순한 지식을 넘어 실제 업무 흐름에 녹아들게 됩니다.

그 결과, 단순히 문서를 빨리 만드는 것이 아니라 **더 나은 제품 의사결정**을 내릴 수 있게 됩니다.

## 작동 방식 (스킬)

**스킬(Skills)**은 이 저장소의 핵심 단위입니다. 각 스킬은 AI에게 특정 PM 작업에 필요한 도메인 지식, 분석 프레임워크 또는 가이드된 워크플로우를 제공합니다.

스킬은 관련 대화 맥락에서 자동으로 로드되거나, 필요한 경우 직접 스킬 파일을 참조하여 사용할 수 있습니다.

## 설치 및 사용 방법

### 웹에서 사용하기: claude.ai

- 등록: claude.ai > Customize > 스킬 메뉴에서 다운로드 받은 스킬(SKILL.md 파일 또는 전체 zip파일)을 등록합니다.
- 사용: Claude 채팅에서 관련된 업무 수행시 자동으로 skill이 적용됩니다.

### AI Coding 툴에서 사용하기

- 원하는 프로젝트(또는 글로벌)의 .claude/skills/ 폴더(Antigravity의 경우 .agent/skills/)에 GitHub에서 받은 스킬 폴더를 붙여 넣습니다.
- 클로드코드가 스스로 Skill을 활용합니다. 스킬 활용을 강제할때는, 커맨드(/스킬이름)을 선택합니다.

---

## 제공되는 스킬 카테고리

### 1. 제품 발견 (pm-product-discovery)

지속적인 제품 발견: 아이디어 구상, 실험, 가설 검증, 기능 우선순위 지정, 기회-솔루션 트리(OST), 고객 인터뷰 분석 등.

### 2. 제품 전략 (pm-product-strategy)

제품 전략, 비전, 비즈니스 모델, 가격 책정 및 거시 환경 분석. 비전 수립부터 경쟁 환경 분석까지의 전략 도구 모음.

### 3. 제품 실행 (pm-execution)

일일 제품 관리 업무: PRD 작성, OKR 수립, 로드맵 관리, 스프린트 계획, 회고, 출시 노트 작성, 사전 부검(Pre-mortem), 이해관계자 관리 등.

### 4. 시장 조사 (pm-market-research)

사용자 조사 및 경쟁사 분석: 페르소나, 세그멘테이션, 여정 지도, 시장 규모 추정, 피드백 분석 등.

### 5. 데이터 분석 (pm-data-analytics)

PM을 위한 데이터 분석: SQL 쿼리 생성, 코호트 분석, A/B 테스트 분석 등.

### 6. 시장 진입 전략 (pm-go-to-market)

GTM 전략: 거점(Beachhead) 세그먼트, 이상적인 고객 프로필(ICP), 메시징, 성장 루프, GTM 모션 등.

### 7. 마케팅 및 성장 (pm-marketing-growth)

제품 마케팅 및 성장: 마케팅 아이디어, 포지셔닝, 가치 제안, 제품 네이밍, 북극성 지표(North Star Metric) 등.

### 8. PM 툴킷 (pm-toolkit)

핵심 업무 외 유틸리티: 이력서 검토, 법률 문서 초안(NDA 등), 맞춤법 및 논리 검토 등.

---

## 참고 문헌

이 저장소의 스킬들은 다음 전문가들의 방법론을 바탕으로 제작되었습니다:

- Teresa Torres — *Continuous Discovery Habits*
- Marty Cagan — *INSPIRED* 및 *TRANSFORMED*
- Alberto Savoia — *The Right It*
- Dan Olsen — *The Lean Product Playbook*
- Roger L. Martin — *Playing to Win*
- Ash Maurya — *Running Lean*
- Strategyzer — *Business Model Generation* 및 *Value Proposition Design*
- Christina Wodtke — *Radical Focus*
- Anthony W. Ulwick — *Jobs to Be Done*
- Alistair Croll & Benjamin Yoskovitz — *Lean Analytics*
- Sean Ellis — *Hacking Growth*
- Maja Voje — *Go-To-Market Strategist*

## 라이선스

MIT — 상세 내용은 [LICENSE](LICENSE) 파일을 참조하세요.
Copyright (c) 2026 황진수(Korean Translation)
