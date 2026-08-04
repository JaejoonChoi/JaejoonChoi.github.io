---
layout: archive
title: "Project Lists & Experiences"
permalink: /project/
author_profile: true
redirect_from:
  - /project
---

{% include base_path %}


**Projects**
----

**Project 2.** 부직포를 이용한 다양한 용도의 매트, 카펫 및 벽지 등에 적용하기 위한 바인더 및 부직포 첨가제 개발
- `With:` Bokwang Industry Co., Ltd. / 2024.09 - 2024.10
- `Period of affiliation:` Kumoh National Institute of Technology

<br/>

**Project 1.** 공중 유·무인 복합체계와 상호운용성을 고려한 스텔스 투사체 개발(Developing stealth projectiles for interoperability with airborne manned and unmanned teaming systems)
- `With:` Defense Acquisition Program Administration (DAPA) / 2024.05 ~ 2024.08
- `Period of affiliation:` Kumoh National Institute of Technology


<br/>
<br/>


**Side Projects**
----
**Side Project 11.** [LLM Textual Gradient Process Discovery Model](https://github.com/JaejoonChoi/Diagtextgrad_LLM-Process-Discovery)
- `Role:` Individual
- `Period:` Individual Term project conducted in the Process Mining Lecture at KyungHee University, 1st Semester 2026, 2026.03 ~ 2026.07
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. We designed DiagTextGrad, an iterative process discovery framework utilizing PM4Py and TextGrad to automate the entire loop from model discovery through diagnosis to revision, addressing the limitation of one-shot algorithm selection where the inductive baseline on our target log reached 0.9990 fitness but only 0.0825 precision — an overly permissive "flower" model that accepts almost any behavior.
  1. We proposed a Diagnosis Agent that translates the four quality dimensions — fitness, precision, generalization, and simplicity — into natural-language assessments of flower-model and spaghetti-model risk, moving beyond fixed metric thresholds to reason about which weakness should be targeted next and at what structural cost.
  1. We implemented an Improvement stage built on TextGrad and served by a locally hosted Gemma-4-31B-it endpoint, in which the LLM-generated proposal itself becomes the optimized parameter: a TextLoss critic and textual gradient descent backpropagate natural-language feedback over a two-level action space spanning miner hyperparameters (algorithm, noise/dependency/AND/loop thresholds) and directly-follows edge removals.
  1. By integrating a Selection stage that enforces hard guardrails (fitness ≥ 0.80, precision ≥ 0.10, simplicity ≥ 0.50) and ranks feasible candidates by a composite score, together with edge-protection rules and a rule-based fallback for malformed or repeated proposals, we ensured that every accepted model remains structurally valid under a robust retry mechanism.
  1. Through this approach, across 50 iterations on a real manufacturing event log (4,543 events, 225 cases, 55 activities), we improved precision 8-fold from 0.0825 to 0.6696 while preserving fitness at 0.9343 and slightly improving simplicity, demonstrating that LLMs deliver the most value in process mining not as autonomous model builders but as proposal engines embedded within a strict validation loop.

  </div>
  </details>

<br/>

**Side Project 10.** [CRM Message Generation System](https://github.com/jaejunchoe/2026-Amore-Pacific-AI-Innovation-Challenge)
- `Role:` Team Member
- `Period:` 2026-Amore-Pacific-AI-Innovation-Challenge, 2025.12 ~ 2026.01
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. We designed a Multi-Agent CRM message generation system utilizing LangGraph to automate the entire process from persona understanding to message creation, addressing the current "content bottleneck" where manual message creation fails to keep pace with rapid targeting capabilities.
  1. We proposed a Persona Analyzer that conducts in-depth analysis of psychological purchase motivations based on 8 core beauty segments, moving beyond simple demographic analysis to understand the customer's context.
  1. We implemented a Product Matcher using a ChromaDB-based RAG pipeline, converting 2,753 original Amorepacific product data points into 516 core product categories to perform semantic matching aligned with the persona's skin concerns and brand information.
  1. By integrating a Message Generator that applies brand-specific tone and manner, and a Quality Checker that validates character limits and predicts CTR, we ensured the generation of high-quality, optimal CRM messages with a robust retry and fallback mechanism.
  1. Through this approach, we expect to significantly improve email open rates (+150~194%) and CTR (+150~192%) while reducing message generation time by over 95%, ultimately maximizing CRM operational efficiency and transforming marketers into strategic designers.

  </div>
  </details>

<br/>

**Side Project 9.** [Convex Optimization-Based Municipal Parking Lot Recommendation System in Seoul](https://github.com/jaejunchoe/convex_25_kyunghee)
- `Role:` Team Member
- `Period:` Term project conducted in the Convex Optimization Lecture at KyungHee University, 2st Semester 2025, 2025.09 ~ 2025.12
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. To resolve the issues of unbalanced utilization rates and parking shortages in Seoul's municipal parking lots, we designed a convex optimization-based dynamic parking recommendation AI agent that allocates the optimal parking lot by reflecting real-time urban data.
  1. We proposed an objective function that simultaneously minimizes parking lot congestion, user travel distance, and parking fees. Additionally, we prevented demand concentration at specific parking lots by applying capacity overflow prevention and an upper bound constraint on congestion ($\rho_{max}$).
  1. We implemented a framework that assigns the optimal parking lot utilizing the CVXPY solver, and integrated a feature where an LLM dynamically recommends hyperparameter weights ($\alpha, \beta, \gamma$) based on real-time situational prompts, such as city festivals or events.
  1. Through this approach, we achieved superior performance across all metrics compared to the conventional Greedy algorithm—including improvements in congestion (+8.2%, +7.5%), parking costs (+4%, +5.8%), and travel distance (+0.2%, +0.8%) for weekdays and weekends, respectively. Furthermore, we demonstrated that this system can effectively alleviate users' parking search time and stress while guaranteeing a global optimal solution.

  </div>
  </details>

<br/>

🥉**Side Project 8.** [CGAFuzz: Curriculum-Guided Adaptive Fuzzing Framework (Combining AFL++ with curriculum learning, EMA-based adaptive mutation, and optional LLM-powered seed generation)](https://github.com/HyeonjongJang/CGAFuzz)
- `Role:` Team Member
- `Period:` 2025 AI-Powered Vulnerability Discovery System Competition, 2025.09 ~ 2025.10
- 🏆`Prize:` [Excellence Prize](/images/AI를_활용한_취약점_발굴_시스템_공모전_상장_ver01.jpg), Chairperson of the IT Platform Safety Research Group, <strong>KRW 2,000,000</strong>
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. We designed a three-phase progression strategy based on JSON validation success rates using Parse-Rate Driven Curriculum Learning.
  1. We proposed EMA-Based Adaptive Mutation, a lightweight and real-time operator scheduling mechanism that learns mutations capable of discovering new paths.
  1. We implemented Plateau Detection to automatically identify coverage stagnation and integrated optional LLM support to generate diverse initial seeds.
  1. By presenting a novel approach for structured input fuzzing via Parse-Rate Driven Curriculum Learning, Lightweight EMA-Based Scheduling, and an Automatic Phase Transition Mechanism, we demonstrated suitability for real-time high-throughput fuzzing and achieved synergy between parse-rate phases and coverage monitoring.
  1. Through this approach, we demonstrated superior performance in both code coverage (+4.03%) and execution speed (+6.50%) compared to standard AFL++, significantly enhancing the efficiency of vulnerability analysis for software with complex structures.

  </div>
  </details>

<br/>

🥈**Side Project 7.** RAG-FSR(Retrieval Augmented Generation-Food Science Research): 자연어 처리와 검색 증강 생성을 통한 식품 연구 저널 분류 언어 모델(A Language Model for Classifying Food Research Journals using Natural Language Processing and Retrieval-Augmented Generation)
- `Role:` Team Member
- `Period:` Data Analysis Sector conducted in 2025 Korea Food Research Institute Food Data Analysis and Utilization Competition, 2025.06 ~ 2025.07
- 🏆`Prize:` [Top Excellence Prize](/images/한국식품연구원_상장1.jpg), President from President of Korea Food Research Institute (KFRI), <strong>KRW 500,000</strong>
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. As the volume of academic data in science and technology rapidly increases, researchers are facing difficulties in searching for prior studies and classifying content due to the limitations of existing keyword-based search systems.
  1. To address this problem, we propose and implement RAG-FSR (Retrieval-Augmented Generation for Food Science Research), a language model specialized for the food research domain that utilizes Retrieval-Augmented Generation (RAG) technology.
  1. The results showed that RAG-FSR achieved an accuracy of 0.960, particularly in the multi-keyword classification task. Furthermore, on the exact-match accuracy metric for abstract generation, our model performed approximately 4-9 times better than the baseline models.
  1. This empirically demonstrates that the proposed model effectively mitigates the hallucination phenomenon common in large language models and can function as a highly accurate and reliable information classification and retrieval system for food science research data.

  </div>
  </details>

<br/>

**Side Project 6.** [Vision Transformer와 유사도 기반 반도체 혼합 결합 유형 예측(Prediction of Mixed Defect Types in Semiconductors Using Vision Transformer and Similarity-Based Methods)](https://github.com/jaejunchoe/2024-1_Capstone-Design)
- `Role:` Individual
- `Period:` Individual Project conducted in a Capstone Design Lecture under the supervision of Prof. Young-Sil Lee at Kumoh National Institute of Technology, 1st Semester 2024 , 2024.03 ~ 2024.05
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. The goal is to predict dual defect types in data using only single defect data.
  1. Two models based on Vision Transformers and KNN algorithms were designed, using Euclidean and Gaussian distance calculation methods for comparative analysis.
  1. Prediction of dual defect types involving 'Edge_Loc' showed higher accuracy than previous studies using CNN, but overall performance was not satisfactory.

  </div>
  </details>


<br/>

🥇**Side Project 5.** [EG(Eco Gumi)-Service: 에너지 효율성 및 지속 가능한 에너지 사용을 위한 통합 플랫폼(Integrated Platform for Energy Efficiency and Sustainable Energy Use)](https://github.com/jaejunchoe/2023-Gumi-Industrial-Complex-Energy-Self-Sufficiency-Datathon)
- `Role:` Team Member
- `Period:` Service Sector conducted in 2023 Gumi Industrial Complex Energy Self-Sufficiency Datathon, 2023.09 ~ 2023.12
- 🏆`Prize:` [Grand Prize](/images/구미산단_데이터톤.jpg), President from Korea Electric Power Corporation(KEPCO), <strong>KRW 4,000,000</strong>
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. Developed a service idea(EG-Service). <br/>
  1. Analyzing the correlations in hourly usage data to identify past times with high correlation to past power usage and conducting time series clustering on the daily usage patterns of power consuming companies. <br/>
  1. Utilizing various algorithmic models such as Linear Regression, LSTM, and Ensemble Methods (Voting, Stacking, etc.) to derive R-squared and MAE. <br/>
  1. Proposing features for visualizing energy usage and policy notification services, and creating a Service Blueprint and user behavior simulation map to refine the service ideas.

  </div>
  </details>

<br/>

🥈**Side Project 4.** 대학 발전을 위한 정책 아이디어(A Policy Idea For University Development)
- `Role:` Team Leader
- `Period:` In-Campus Contest conducted in the Policy Idea Contest for University Development at Kumoh National Institute of Technology, 2023.09 ~ 2023.11
- 🏆`Prize:` [Second Prize](/images/금오공대_정책_공모전_우수.jpg), University President's Award from Kumoh National Institute of Technology, <strong>KRW 500,000</strong>
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. We will establish a “School of Liberal Studies” for undergraduate students to strengthen their convergence capabilities and expand opportunities for major exploration.
  1. We will improve the course evaluation system to facilitate better communication between students and professors.
  1. Through initiatives like the “Alumni School Visit Program” and a nationwide high school promotion tour, we will attract outstanding students from other regions.
  1. Following the example of Duksung Women’s University, we aim to increase students' satisfaction with major selection by offering a major exploration period, while enhancing the university’s global and creative brand value.
  1. Through these initiatives, we aim to achieve enhanced competitiveness, innovative education, and a stronger university brand for Kumoh National Institute of Technology.

  </div>
  </details>

<br/>

**Side Project 3.** [서울시의 노인 돌봄 센터 제안과 AI를 활용한 최적의 위치 선정 및 제안(Proposed elder care centers in Seoul and identified optimal locations using AI)](https://github.com/jaejunchoe/2023-Seoul-Artificial-Intelligence-Idea-Challenge)
- `Role:` Team Member
- `Period:` Contest conducted in the 2023 Seoul Artificial Intelligence Idea Challenge, 2023.08 ~ 2023.10
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. Proposal for 'Elderly Care Centers' (ECC) and Selection of Optimal Locations Based on Data.
  1. By utilizing data on population and the number of welfare facilities in each region, we conducted clustering to select areas that need to be converted into ECC based on the proportional and inversely proportional relationships of the compared data.
  1. Clustering was performed using DBSCAN, and the hyperparameters were derived through GridSearch.
  1. As a result, we identified Nowon-gu, Gangseo-gu, Yangcheon-gu, Songpa-gu, and Seongbuk-gu as areas urgently requiring conversion into ECCs.

  </div>
  </details>

<br/>

**Side Project 2.** [2024년 FA(자유계약선수) 자격을 갖춘 KBO 선수들의 연봉 예측(Salary prediction for KBO players eligible for FA (Free Agent) in 2024)](https://github.com/jaejunchoe/Prediction-of-2024-KBO-Players-Free-Agency-Salaries)
- `Role:` Team Member & Presenter
- `Period:` Term project conducted in the Machine Learning Lecture at Kumoh National Institute of Technology, 1st Semester 2023, 2023.05 ~ 2023.06
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. Collected performance metrics for KBO players who signed FA contracts from 2019 to 2023.
  1. Analyzed the correlation between performance metrics and salaries for pitchers and batters.
  1. Created a model using RandomForestRegressor with performance metrics that had a correlation of 0.5 or higher.

  </div>
  </details>

<br/>

📄**Side Project 1.** [쇼핑카트의 불편한 점을 해결하는 새로운 아이디어 발굴 및 디자인권 등록(Developing innovative ideas to address the inconveniences of shopping carts and registering design patent)](https://doi.org/10.8080/3020230035785.M001)
- `Role:` Team Member & Presenter
- `Period:` Term project conducted in the Product·System Design Lecture at Kumoh National Institute of Technology, 1st Semester 2023, 2023.04 ~ 2023.06
- 📄`Patent:` A Design Right with the Korea Intellectual Property Rights Information Service (KIPRIS) under [KR-Registration No. 3012568290000](https://doi.org/10.8080/3020230035785.M001)
- <details><summary><code>Contents:</code> (Click to expand)</summary>
  <div markdown="1">

  1. It was designed so that the front panel can rotate open around a hinge axis while the cart is adjusted to match the height of the checkout counter.
  1. A holder for a mobile phone and beverage container was added to the handle, and the front panel can be opened and closed by rotating around the hinge axis for easy access to items. Additionally, a height-adjustment function was included by using a hydraulic lever to vary the distance between the wheels.

  </div>
  </details>