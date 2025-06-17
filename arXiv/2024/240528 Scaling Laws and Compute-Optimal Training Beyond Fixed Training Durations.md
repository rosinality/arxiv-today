https://arxiv.org/abs/2405.18392

*Scaling Laws and Compute-Optimal Training Beyond Fixed Training Durations* (Alexander Hägele, Elie Bakouch, Atli Kosson, Loubna Ben Allal, Leandro Von Werra, Martin Jaggi)

> Scale has become a main ingredient in obtaining strong machine learning models. As a result, understanding a model's scaling properties is key to effectively designing both the right training setup as well as future generations of architectures. In this work, we argue that scale and training research has been needlessly complex due to reliance on the cosine schedule, which prevents training across different lengths for the same model size. We investigate the training behavior of a direct alternative - constant learning rate and cooldowns - and find that it scales predictably and reliably similar to cosine. Additionally, we show that stochastic weight averaging yields improved performance along the training trajectory, without additional training costs, across different scales. Importantly, with these findings we demonstrate that scaling experiments can be performed with significantly reduced compute and GPU hours by utilizing fewer but reusable training runs.

요즘 유행하는 Constant LR + Cooldown 스케줄을 Scaling Law 추정에 활용한 방법이네요. 코사인 스케줄을 쓴다면 모델 크기/학습량에 따라 새로운 모델을 학습시켜야 하죠. 그런데 Constant LR을 쓴다고 하면 같은 모델을 추가 학습한 다음 Cooldown을 시키면 되기에 재활용을 할 수 있습니다.

사실 DeepSeek LLM (https://arxiv.org/abs/2401.02954) 에서도 사용한 방법이고 MiniCPM에서도 Scaling Law 추정에 활용했을 것 같네요. (https://shengdinghu.notion.site/MiniCPM-Unveiling-the-Potential-of-End-side-Large-Language-Models-d4d3a8c426424654a4e80e42a711cb20) 

#scaling-law

# Links

[[240105 DeepSeek LLM.md]]