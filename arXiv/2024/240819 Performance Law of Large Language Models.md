https://arxiv.org/abs/2408.09895

*Performance Law of Large Language Models* (Chuhan Wu, Ruiming Tang)

> Guided by the belief of the scaling law, large language models (LLMs) have achieved impressive performance in recent years. However, scaling law only gives a qualitative estimation of loss, which is influenced by various factors such as model architectures, data distributions, tokenizers, and computation precision. Thus, estimating the real performance of LLMs with different training settings rather than loss may be quite useful in practical development. In this article, we present an empirical equation named "Performance Law" to directly predict the MMLU score of an LLM, which is a widely used metric to indicate the general capability of LLMs in real-world conversations and applications. Based on only a few key hyperparameters of the LLM architecture and the size of training data, we obtain a quite accurate MMLU prediction of various LLMs with diverse sizes and architectures developed by different organizations in different years. Performance law can be used to guide the choice of LLM architecture and the effective allocation of computational resources without extensive experiments.

모델 학습 규모로 MMLU 예측하기. 다들 한 번 해보는 작업 같네요. 뭔가 함수의 형태가 작위적인 느낌은 있긴 합니다만 예측은 그럴 듯 하네요. 레이어의 수, 히든 임베딩 차원, FFN의 크기, 학습 토큰 수, (MoE의 경우) Activated Parameter. 수많은 차이에도 결국 Scaling Law로 회귀한다는 것이 재미있습니다. 과연 Scaling Law는 속일 수 없는 것인지.

#scaling-law 