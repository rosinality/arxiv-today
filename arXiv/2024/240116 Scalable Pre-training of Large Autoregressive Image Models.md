https://arxiv.org/abs/2401.08541

*Scalable Pre-training of Large Autoregressive Image Models* (Alaaeldin El-Nouby, Michal Klein, Shuangfei Zhai, Miguel Angel Bautista, Alexander Toshev, Vaishaal Shankar, Joshua M Susskind, Armand Joulin)

> This paper introduces AIM, a collection of vision models pre-trained with an autoregressive objective. These models are inspired by their textual counterparts, i.e., Large Language Models (LLMs), and exhibit similar scaling properties. Specifically, we highlight two key findings: (1) the performance of the visual features scale with both the model capacity and the quantity of data, (2) the value of the objective function correlates with the performance of the model on downstream tasks. We illustrate the practical implication of these findings by pre-training a 7 billion parameter AIM on 2 billion images, that achieves 84.0% on ImageNet-1k with a frozen trunk. Interestingly, even at this scale, we observe no sign of saturation in performance, suggesting that AIM potentially represents a new frontier for training large-scale vision models. The pre-training of AIM is similar to the pre-training of LLMs, and does not require any image-specific strategy to stabilize the training at scale.

패치 기반의 심플한 Autoregressive 학습으로 Vision 백본 만들기. 모델들이 데이터셋도 모델 크기도 평가 세팅도 달라서 비교가 참 어렵긴 하지만 일단 된다는 것 & 더 큰 규모에서도 될 것 같다는 것을 보면 되지 않을까 싶습니다. Multitask 통합과 (https://arxiv.org/abs/2312.00785) Generation에 대한 고려가 계속해서 흥미로운 주제일 듯 싶네요.

#autoregressive_model #vision #backbone

# Links

[[231201 Sequential Modeling Enables Scalable Learning for Large Vision Models.md]]