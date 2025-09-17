https://arxiv.org/abs/2508.00180

*EMA Without the Lag: Bias-Corrected Iterate Averaging Schemes* (Adam Block, Cyril Zhang)

> Stochasticity in language model fine-tuning, often caused by the small batch sizes typically used in this regime, can destabilize training by introducing large oscillations in generation quality. A popular approach to mitigating this instability is to take an Exponential moving average (EMA) of weights throughout training. While EMA reduces stochasticity, thereby smoothing training, the introduction of bias from old iterates often creates a lag in optimization relative to vanilla training. In this work, we propose the Bias-Corrected Exponential Moving Average (BEMA), a simple and practical augmentation of EMA that retains variance-reduction benefits while eliminating bias. BEMA is motivated by a simple theoretical model wherein we demonstrate provable acceleration of BEMA over both a standard EMA and vanilla training. Through an extensive suite of experiments on Language Models, we show that BEMA leads to significantly improved convergence rates and final performance over both EMA and vanilla training in a variety of standard LM benchmarks, making BEMA a practical and theoretically motivated intervention for more stable and efficient fine-tuning.

EMA를 사용해서 최적화 궤적을 안정화하면 최적화의 속도가 지연되게 되는데, 이 지연을 없애려고 한 시도.

Using EMA to stabilize optimization trajectories induces a lag in the optimization. This work tried to eliminate it.

#optimization 