https://arxiv.org/abs/2504.10478

*Weight Ensembling Improves Reasoning in Language Models* (Xingyu Dang, Christina Baek, Kaiyue Wen, Zico Kolter, Aditi Raghunathan)

> We investigate a failure mode that arises during the training of reasoning models, where the diversity of generations begins to collapse, leading to suboptimal test-time scaling. Notably, the Pass@1 rate reliably improves during supervised finetuning (SFT), but Pass@k rapidly deteriorates. Surprisingly, a simple intervention of interpolating the weights of the latest SFT checkpoint with an early checkpoint, otherwise known as WiSE-FT, almost completely recovers Pass@k while also improving Pass@1. The WiSE-FT variant achieves better test-time scaling (Best@k, majority vote) and achieves superior results with less data when tuned further by reinforcement learning. Finally, we find that WiSE-FT provides complementary performance gains that cannot be achieved only through diversity-inducing decoding strategies, like temperature scaling. We formalize a bias-variance tradeoff of Pass@k with respect to the expectation and variance of Pass@1 over the test distribution. We find that WiSE-FT can reduce bias and variance simultaneously, while temperature scaling inherently trades-off between bias and variance.

SFT 초반과 후반의 Weight에 대한 Averaging으로 샘플 다양성의 감소를 억제할 수 있다는 결과. 다양성의 중요성을 고려하면 중요한 트릭이 될 듯 하네요.

<english>
A result suggesting we can suppress the decline in sample diversity by averaging the weight from early and late stage of SFT. As diversity is crucial, it can became important tricks.
</english>

#ensemble #reasoning 