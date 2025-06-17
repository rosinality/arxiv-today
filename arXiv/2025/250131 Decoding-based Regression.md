https://arxiv.org/abs/2501.19383

*Decoding-based Regression* (Xingyou Song, Dara Bahri)

> Language models have recently been shown capable of performing regression tasks wherein numeric predictions are represented as decoded strings. In this work, we provide theoretical grounds for this capability and furthermore investigate the utility of causal auto-regressive sequence models when they are applied to any feature representation. We find that, despite being trained in the usual way - for next-token prediction via cross-entropy loss - decoding-based regression is as performant as traditional approaches for tabular regression tasks, while being flexible enough to capture arbitrary distributions, such as in the task of density estimation.

회귀 문제에 대해 각 자릿수의 값을 하나씩 생성하는 형태의 Autoregression으로 대응.

<english>
A method for doing regression with autoregressive models by generating each digits as a token.
</english>

#autoregressive-model 