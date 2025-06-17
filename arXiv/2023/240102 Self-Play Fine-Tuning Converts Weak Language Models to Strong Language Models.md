https://arxiv.org/abs/2401.01335

Self-Play Fine-Tuning Converts Weak Language Models to Strong Language Models (Zixiang Chen, Yihe Deng, Huizhuo Yuan, Kaixuan Ji, Quanquan Gu)

SFT를 하더라도 SFT 데이터와 모델 퍼포먼스 사이의 갭이 있으니 SFT 데이터를 Positive, LM 샘플을 Negative로 해서 DPO스러운 학습을 하는 방법이네요. Gold Standard를 설정하고 거기에 맞추는 쪽으로 튜닝하는 것은 Adversarial Preference Optimization (https://arxiv.org/abs/2311.08045) 의 시도와 비슷해 보이기도 합니다.

#instruction-tuning

# Links

[[231114 Adversarial Preference Optimization.md]]