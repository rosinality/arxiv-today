https://arxiv.org/abs/2503.13431

*Measuring In-Context Computation Complexity via Hidden State Prediction* (Vincent Herrmann, Róbert Csordás, Jürgen Schmidhuber)

> Detecting when a neural sequence model does "interesting" computation is an open problem. The next token prediction loss is a poor indicator: Low loss can stem from trivially predictable sequences that are uninteresting, while high loss may reflect unpredictable but also irrelevant information that can be ignored by the model. We propose a better metric: measuring the model's ability to predict its own future hidden states. We show empirically that this metric -- in contrast to the next token prediction loss -- correlates with the intuitive interestingness of the task. To measure predictability, we introduce the architecture-agnostic "prediction of hidden states" (PHi) layer that serves as an information bottleneck on the main pathway of the network (e.g., the residual stream in Transformers). We propose a novel learned predictive prior that enables us to measure the novel information gained in each computation step, which serves as our metric. We show empirically that our metric predicts the description length of formal languages learned in-context, the complexity of mathematical reasoning problems, and the correctness of self-generated reasoning chains.

모델에서 일어나는 연산의 복잡성을 측정하려는 시도. 토큰 Perplexity는 그저 노이즈 때문에 높은 것일 수도 있으니 Next Hidden State에 대한 예측으로 측정하겠다는 시도입니다. Hidden State에 대한 예측이라고 하니 Test Time Train 연구들도 생각나네요. (https://arxiv.org/abs/2407.04620, https://arxiv.org/abs/2501.00663)

<english>
An attempt to measure complexity of computation happening inside th e model. Token perplexity could be high just due to noises, they tried to estimate it by predicting next hidden states. For hidden state prediction, it reminds me researches on test time train (https://arxiv.org/abs/2407.04620, https://arxiv.org/abs/2501.00663).
</english>

#mechanistic-interpretation 