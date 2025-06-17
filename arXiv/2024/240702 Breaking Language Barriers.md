https://arxiv.org/abs/2407.02118

*Breaking Language Barriers: Cross-Lingual Continual Pre-Training at Scale* (Wenzhen Zheng, Wenbo Pan, Xu Xu, Libo Qin, Li Yue, Ming Zhou)

> In recent years, Large Language Models (LLMs) have made significant strides towards Artificial General Intelligence. However, training these models from scratch requires substantial computational resources and vast amounts of text data. In this paper, we explore an alternative approach to constructing an LLM for a new language by continually pretraining (CPT) from existing pretrained LLMs, instead of using randomly initialized parameters. Based on parallel experiments on 40 model sizes ranging from 40M to 5B parameters, we find that 1) CPT converges faster and saves significant resources in a scalable manner; 2) CPT adheres to an extended scaling law derived from Hoffmann et al. (2022) with a joint data-parameter scaling term; 3) The compute-optimal data-parameter allocation for CPT markedly differs based on our estimated scaling factors; 4) The effectiveness of transfer at scale is influenced by training duration and linguistic properties, while robust to data replaying, a method that effectively mitigates catastrophic forgetting in CPT. We hope our findings provide deeper insights into the transferability of LLMs at scale for the research community.

새로운 언어에 대한 Continual Pretraining Scaling Law. 베이스 모델이 강력한 쪽이 Continual Pretraining에 더 많은 데이터를 쓰는 것보다 효율적이라는 것, 5 - 30% 정도의 원 언어 데이터를 섞어주는 것이 효과적이라는 결론. 원 언어에 대한 데이터를 이 정도 섞는 것은 Continual Pretraining에 대한 레시피 탐색에서 발견한 것과 비슷하네요. (https://arxiv.org/abs/2403.08763)

#continual-learning #pretraining #multilingual

# Links

[[240313 Simple and Scalable Strategies to Continually Pre-train Large Language Models.md]]