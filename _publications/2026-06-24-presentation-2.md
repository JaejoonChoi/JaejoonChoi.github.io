---
title: "[PT] JSON 퍼징에서 뮤테이터 구조에 따른 CmpLog의 차별적 효용 분석: Semantic-Aware 변이와 바이트 수준 변이의 비교"
collection: publications
category: conferences
permalink: /publication/2026-06-24-presentation-2
excerpt: '`Keywords: JSON Fuzzing, CmpLog, Semantic-Aware Mutation, Byte-level Mutation, AFL++, Software Security` <br/> 🏆 Best Paper Award — Information Security & High-Reliability Computing at the Korean Institute of Information Scientistis and Engineers'
date: 2026-06-24
venue: '한국컴퓨터종합학술대회(KCC2026)'
#paperurl: ''
citation: '장현종, <strong>최재준</strong>, 김영훈*. JSON 퍼징에서 뮤테이터 구조에 따른 CmpLog의 차별적 효용 분석: Semantic-Aware 변이와 바이트 수준 변이의 비교. 2026 한국정보과학회 학술발표논문집, 2026'
---

# Abstract
퍼징(Fuzzing)은 소프트웨어 취약점을 식별하는 효과적인 동적 분석 기법이나, JSON과 같이 엄격한 문법이 요구되는 구조화된 입력에서는 기존의 무작위 바이트 수준(byte-level) 변이가 유효성 함정 문제를 발생시킨다. 이를 해결하기 위해 입력 구조를 유지하는 의미 인식(semantic-aware) 변이 기법이 제안되었으나, 이러한 기법과 CmpLog와 같은 동적 비교 계측 기법을 결합했을 때의 상호작용 및 상보성을 정량적으로 분석한 시도는 부족했다. 이에 본 논문에서는 11개의 JSON 인식 연산자와 파싱 비율(parse-rate) 주도의 3단계 커리큘럼 학습을 적용한 맞춤형 뮤테이터 CGAFuzz를 제안한다. CGAFuzz는 함수 호출 오버헤드로 인해 단기 실행에서의 절대 커버리지는 상대적으로 낮았으나 실행 당 에지 발견 측면에서는 월등한 효율성을 입증하였다. 특히, 의미론적 연산자가 이스케이프 시퀀스 등의 비표준 토큰을 무작위로 탐색하지 못하여 발생하는 바이트 수준의 사각지대를 CmpLog의 동적 사전 주입을 통해 효과적으로 보완하였다. 결과적으로 CmpLog 결합 시 기존 모델과의 커버리지 격차가 평균 41~60% 일관되게 감소하였으며, 이는 문법 및 의미 인식 퍼저 설계 시 동적 분석 기법의 결합이 필수적인 보완재임을 증명한다.  <br/>


Fuzzing is an effective dynamic analysis technique for identifying software vulnerabilities; however, for structured inputs that require strict syntax, such as JSON, conventional random byte-level mutations often lead to the validity trap problem. To address this, semantic-aware mutation techniques that preserve the input structure have been proposed. Nevertheless, there has been a lack of attempts to quantitatively analyze the interaction and complementarity when combining these techniques with dynamic comparison instrumentation methods like CmpLog. Accordingly, in this paper, we propose CGAFuzz, a custom mutator that incorporates 11 JSON-aware operators and a parse-rate-driven three-stage curriculum learning approach. Although CGAFuzz exhibited relatively lower absolute coverage in short-term executions due to function call overhead, it demonstrated superior efficiency in terms of edge discovery per execution. In particular, the dynamic dictionary injection of CmpLog effectively compensated for the byte-level blind spots caused by the inability of semantic operators to randomly explore non-standard tokens, such as escape sequences. Consequently, the integration of CmpLog consistently reduced the coverage gap with baseline models by an average of 41% to 60%. This demonstrates that integrating dynamic analysis techniques is an essential complementary approach when designing syntax- and semantic-aware fuzzers.

<br/>


