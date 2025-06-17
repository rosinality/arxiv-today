https://arxiv.org/abs/2402.02992

*Decoding-time Realignment of Language Models* (Tianlin Liu, Shangmin Guo, Leonardo Bianco, Daniele Calandriello, Quentin Berthet, Felipe Llinares, Jessica Hoffmann, Lucas Dixon, Michal Valko, Mathieu Blondel)

> Aligning language models with human preferences is crucial for reducing errors and biases in these models. Alignment techniques, such as reinforcement learning from human feedback (RLHF), are typically cast as optimizing a tradeoff between human preference rewards and a proximity regularization term that encourages staying close to the unaligned model. Selecting an appropriate level of regularization is critical: insufficient regularization can lead to reduced model capabilities due to reward hacking, whereas excessive regularization hinders alignment. Traditional methods for finding the optimal regularization level require retraining multiple models with varying regularization strengths. This process, however, is resource-intensive, especially for large models. To address this challenge, we propose decoding-time realignment (DeRa), a simple method to explore and evaluate different regularization strengths in aligned models without retraining. DeRa enables control over the degree of alignment, allowing users to smoothly transition between unaligned and aligned models. It also enhances the efficiency of hyperparameter tuning by enabling the identification of effective regularization strengths using a validation dataset.

RLHF 학습 과정에서 KL Penalty 계수를 바꿨을 때의 결과를 재학습 없이 알 수 있을까? SFT 모델과 RLHF 모델의 Logit을 결합하는 것으로 시뮬레이션을 할 수 있다는 결과입니다. RLHF 튜닝 작업에 대해 굉장히 유용한 도구가 될 수 있을 것 같네요.

#rlhf 

Can we know the result of changing KL penalty coefficient of RLHF training without retraining? This study shows that we can simulate it with combining logit of SFT and RLHF models. I think this could be really useful tool for RLHF tuning process.