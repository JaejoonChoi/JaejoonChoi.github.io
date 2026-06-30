---
title: "[PT] 웨이퍼 빈 맵 분류를 위한 Feature-Wise Linear Modulation 기반 조건부 분할 모델"
collection: publications
category: conferences
permalink: /publication/2025-11-06-presentation-1
excerpt: '`Keywords: Deep Learning, Mixed-type Defects Detection & Semantic Segmentation, Disentanglement of Mixed Defects, Feature-wise Linear Modulation (FiLM)`'
date: 2025-11-06
venue: '대한산업공학회 추계학술대회'
#paperurl: ''
citation: '<strong>최재준</strong>, 김영훈*. 웨이퍼 빈 맵 분류를 위한 Feature-Wise Linear Modulation 기반 조건부 분할 모델. 대한산업공학회 추계학술대회 논문집, 2025'
---

# Abstract
반도체 공정이 고도화됨에 따라, 다중 웨이퍼 결함을 정밀하게 분류하는 것의 중요성이 커지고 있습니다. 본 논문은 단일 네트워크를 사용하여 특정 결함을 선택적으로 분할하는 U-Net 기반의 조건부 모델을 제안합니다. 디코더에 Feature-wise Linear Modulation (FiLM) 레이어를 통합함으로써, 모델은 주어진 결함 레이블에 따라 특징 맵을 동적으로 조정하여 해당 결함에 대한 분할 마스크만을 생성합니다. MixedWM38 데이터셋을 이용한 실험 결과는 조건부 결함 분할 및 분류에 있어 우수한 성능을 입증하였습니다. 나아가 2중, 3중, 4중 결함 케이스를 학습 데이터셋에서 체계적으로 배제한 Ablation Study를 수행하였을 때에도, 제안하는 모델은 전체 MixedWM38 데이터셋에 대해 평가 시 가장 우수한 성능을 유지하였습니다. 최종적으로, 본 접근 방식은 복잡한 혼합 유형의 결함 분석을 용이하게 하고 공정 수율 관리를 개선하는 데 기여할 것으로 기대됩니다.   <br/>


As semiconductor processes advance, precisely classifying multiple wafer defects is increasingly important. This paper introduces a U-Net-based conditional model that uses a single network to selectively segment specific defects. By integrating a Feature-wise Linear Modulation (FiLM) layer into the decoder, the model dynamically adjusts its feature maps based on a given defect label, generating a segmentation mask for only that defect. Experimental results on the MixedWM38 dataset demonstrate superior performance in conditional defect segmentation and classification. Furthermore, through ablation studies where double, triple, and quadruple defect cases were systematically excluded from the training set, the proposed model maintained the highest performance when evaluated on the full MixedWM38 dataset. Finally, this approach is expected to facilitate the analysis of complex mixed-type defects and contribute to improved process yield management.

<br/>


