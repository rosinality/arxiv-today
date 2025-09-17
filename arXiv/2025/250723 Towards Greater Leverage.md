https://arxiv.org/abs/2507.17702

*Towards Greater Leverage: Scaling Laws for Efficient Mixture-of-Experts Language Models* (Changxin Tian, Kunlong Chen, Jia Liu, Ziqi Liu, Zhiqiang Zhang, Jun Zhou)

> Mixture-of-Experts (MoE) has become a dominant architecture for scaling Large Language Models (LLMs) efficiently by decoupling total parameters from computational cost. However, this decoupling creates a critical challenge: predicting the model capacity of a given MoE configurations (e.g., expert activation ratio and granularity) remains an unresolved problem. To address this gap, we introduce Efficiency Leverage (EL), a metric quantifying the computational advantage of an MoE model over a dense equivalent. We conduct a large-scale empirical study, training over 300 models up to 28B parameters, to systematically investigate the relationship between MoE architectural configurations and EL. Our findings reveal that EL is primarily driven by the expert activation ratio and the total compute budget, both following predictable power laws, while expert granularity acts as a non-linear modulator with a clear optimal range. We integrate these discoveries into a unified scaling law that accurately predicts the EL of an MoE architecture based on its configuration. To validate our derived scaling laws, we designed and trained Ling-mini-beta, a pilot model for Ling-2.0 series with only 0.85B active parameters, alongside a 6.1B dense model for comparison. When trained on an identical 1T high-quality token dataset, Ling-mini-beta matched the performance of the 6.1B dense model while consuming over 7x fewer computational resources, thereby confirming the accuracy of our scaling laws. This work provides a principled and empirically-grounded foundation for the scaling of efficient MoE models.

굉장한 결과. MoE에 대한 온갖 문제들을 한 번에 해결하는 연구. 일단 MoE가 연산량 증가에 따른 최적 데이터 크기 증가의 비율이 더 높다는 것을 다시 확인하면서 시작.

Efficiency Leverage (Compute Multiplier)에 대한 분석. 연산량과 Activation Sparsity의 증가에 따라 EL이 증가하는 것을 확인. Granularity, Expert Sharing은 최적 지점이 있음. 그 외의 요소에는 큰 영향이 없음.

새삼스럽지만 DeepSeek V3와 (Kimi K2의) 선택이 거의 최적이라는 것이 확인됨.

Impressive results. This resolves various problems around MoE all at once. First it reconfirms that MoE has a higher ratio of optimal data size relative to computational cost compared to dense.

Analysis of Efficiency Leverage (compute multiplier). EL increases with computational cost and activation sparsity. Granularity and expert sharing have optimal points. Other factors don't have much impact.

Not surprisingly, it's confirmed once again that the choices made by DeepSeek V3 and (Kimi K2) are close to optimal.

#moe #scaling-law 