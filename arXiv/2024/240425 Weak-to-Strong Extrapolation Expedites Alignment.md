https://arxiv.org/abs/2404.16792

*Weak-to-Strong Extrapolation Expedites Alignment* (Chujie Zheng, Ziqi Wang, Heng Ji, Minlie Huang, Nanyun Peng)

> Although the capabilities of large language models (LLMs) ideally scale up with increasing data and compute, they are inevitably constrained by limited resources in reality. Suppose we have a moderately trained LLM (e.g., trained to align with human preference) in hand, can we further exploit its potential and cheaply acquire a stronger model? In this paper, we propose a simple method called ExPO to boost LLMs' alignment with human preference. ExPO assumes that a medium-aligned model can be interpolated between a less-aligned (weaker) model, e.g., the initial SFT model, and a better-aligned (stronger) one, thereby directly obtaining this stronger model by extrapolating from the weights of the former two relatively weaker models. On the AlpacaEval 2.0 benchmark, we show that ExPO pushes models trained with less preference data (e.g., 10% or 20%) to reach and even surpass the fully-trained one, without any additional training. Furthermore, ExPO also significantly improves off-the-shelf DPO/RLHF models and exhibits decent scalability across model sizes from 7B to 70B. Our work demonstrates the efficacy of model extrapolation in exploiting LLMs' capabilities, suggesting a promising direction that deserves future exploration.

더 정렬된 모델과 덜 정렬된 모델의 선형 결합으로 중간 정렬 모델을 만들 수 있으니 중간 정렬된 모델과 덜 정렬된 모델의 차이의 반대 방향으로 외삽하면 더 정렬된 모델이 나오지 않을까 하는 아이디어. 재미있네요.

#alignment #model-merge
