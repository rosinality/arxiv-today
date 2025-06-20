https://arxiv.org/abs/2410.18640

*Weak-to-Strong Preference Optimization: Stealing Reward from Weak Aligned Model* (Wenhong Zhu, Zhiwei He, Xiaofeng Wang, Pengfei Liu, Rui Wang)

> Aligning language models (LMs) with human preferences has become a key area of research, enabling these models to meet diverse user needs better. Inspired by weak-to-strong generalization, where a strong LM fine-tuned on labels generated by a weaker model can consistently outperform its weak supervisor, we extend this idea to model alignment. In this work, we observe that the alignment behavior in weaker models can be effectively transferred to stronger models and even exhibit an amplification effect. Based on this insight, we propose a method called Weak-to-Strong Preference Optimization (WSPO), which achieves strong model alignment by learning the distribution differences before and after the alignment of the weak model. Experiments demonstrate that WSPO delivers outstanding performance, improving the win rate of Qwen2-7B-Instruct on Arena-Hard from 39.70 to 49.60, achieving a remarkable 47.04 length-controlled win rate on AlpacaEval 2, and scoring 7.33 on MT-bench. Our results suggest that using the weak model to elicit a strong model with a high alignment ability is feasible.

레퍼런스 모델과 정렬할 모델의 Likelihood의 비율을 정렬된 작은 모델의 Likelihood의 비율과 맞추는 방법으로 정렬하는 방법. 큰 모델에서도 Likelihood의 비율이 지나치게 달라져선 안 된다는 아이디어로 생각할 수 있을 듯 하네요.

<english>
Aligning models by matching ratio of likelihoods of reference models and aligning models, with ratio of small, alignmed models. I think we can think this as regularization that ensures ratio of likelihoods should not be very different even for larger models.
</english>

#alignment 