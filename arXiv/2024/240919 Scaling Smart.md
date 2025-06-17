https://arxiv.org/abs/2409.12903

*Scaling Smart: Accelerating Large Language Model Pre-training with Small Model Initialization* (Mohammad Samragh, Iman Mirzadeh, Keivan Alizadeh Vahid, Fartash Faghri, Minsik Cho, Moin Nabi, Devang Naik, Mehrdad Farajtabar)

> The pre-training phase of language models often begins with randomly initialized parameters. With the current trends in scaling models, training their large number of parameters can be extremely slow and costly. In contrast, small language models are less expensive to train, but they often cannot achieve the accuracy of large models. In this paper, we explore an intriguing idea to connect these two different regimes: Can we develop a method to initialize large language models using smaller pre-trained models? Will such initialization bring any benefits in terms of training time and final accuracy? In this paper, we introduce HyperCloning, a method that can expand the parameters of a pre-trained language model to those of a larger model with increased hidden dimensions. Our method ensures that the larger model retains the functionality of the smaller model. As a result, the larger model already inherits the predictive power and accuracy of the smaller model before the training starts. We demonstrate that training such an initialized model results in significant savings in terms of GPU hours required for pre-training large language models.

작은 모델을 사용해 큰 모델을 초기화하는 전략. 이쪽에서는 레이어를 늘리기보다는 Weight를 복붙해서 너비를 넓히는 쪽으로 했군요. Gopher나 Layer Stacking에서도 비슷한 전략을 찾을 수 있고 (https://arxiv.org/abs/2405.15319) 보통 레이어 증가보다는 효과적이지 않다고 했던 것 같긴 합니다. 이쪽은 결과가 달랐던 이유가 궁금하네요.

#efficient-training

# Links

[[240524 Stacking Your Transformers.md]]