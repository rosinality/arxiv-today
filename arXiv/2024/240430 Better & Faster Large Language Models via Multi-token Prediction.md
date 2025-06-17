https://arxiv.org/abs/2404.19737

*Better & Faster Large Language Models via Multi-token Prediction* (Fabian Gloeckle, Badr Youbi Idrissi, Baptiste Rozière, David Lopez-Paz, Gabriel Synnaeve)

> Large language models such as GPT and Llama are trained with a next-token prediction loss. In this work, we suggest that training language models to predict multiple future tokens at once results in higher sample efficiency. More specifically, at each position in the training corpus, we ask the model to predict the following n tokens using n independent output heads, operating on top of a shared model trunk. Considering multi-token prediction as an auxiliary training task, we measure improved downstream capabilities with no overhead in training time for both code and natural language models. The method is increasingly useful for larger model sizes, and keeps its appeal when training for multiple epochs. Gains are especially pronounced on generative benchmarks like coding, where our models consistently outperform strong baselines by several percentage points. Our 13B parameter models solves 12 % more problems on HumanEval and 17 % more on MBPP than comparable next-token models. Experiments on small algorithmic tasks demonstrate that multi-token prediction is favorable for the development of induction heads and algorithmic reasoning capabilities. As an additional benefit, models trained with 4-token prediction are up to 3 times faster at inference, even with large batch sizes.

바로 다음 토큰 뿐만 아니라 추가로 여러 토큰을 더 예측하도록 학습하는 방법. 사실 이렇게 여러 토큰을 예측하는 방법은 샘플링 속도 가속 측면에서 지속적으로 나오고 있죠. (https://arxiv.org/abs/1811.03115, https://arxiv.org/abs/2401.10774)

이 논문은 여러 토큰을 예측하는 것이 샘플링 가속 뿐만 아니라 성능 자체에도 도움이 될 수 있다는 이야기를 합니다. 작은 모델에서는 손해가 나타나지만 모델이 커지면 오히려 성능이 향상된다는 것이죠. 학습 토큰이 증가하면 향상폭이 감소하는 것 같기도 합니다만 여하간 향상이 나타나는 경우가 있다는 것이 흥미롭네요.

논문에서도 인용하고 있지만 (https://arxiv.org/abs/2403.06963) 다음 토큰만 예측하도록 하는 것이 학습 시그널을 약화시키는 영향이 있을 수 있습니다. 그런 의미에서 마스킹 같은 방법들과 같이 생각해보면 재미있을 듯 하네요.

새로운 학습 Objective는 탐구할 가치가 있는 주제일 듯 합니다. 또한 작은 규모에서는 효과가 있었지만 큰 규모에서 효과가 사라지는 사례들과 반대로 작은 규모에서는 손해였다가 큰 규모에서는 도움이 되는 사례들도 있을 수 있다는 증거가 될 수 있을 듯 하네요.

#pretraining #autoregressive-model

# Links

[[240311 The pitfalls of next-token prediction.md]]