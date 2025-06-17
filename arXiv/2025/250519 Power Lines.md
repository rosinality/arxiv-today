https://arxiv.org/abs/2505.13738

*Power Lines: Scaling Laws for Weight Decay and Batch Size in LLM Pre-training* (Shane Bergsma, Nolan Dey, Gurpreet Gosal, Gavia Gray, Daria Soboleva, Joel Hestness)

> Efficient LLM pre-training requires well-tuned hyperparameters (HPs), including learning rate {\eta} and weight decay {\lambda}. We study scaling laws for HPs: formulas for how to scale HPs as we scale model size N, dataset size D, and batch size B. Recent work suggests the AdamW timescale, B/({\eta}{\lambda}D), should remain constant across training settings, and we verify the implication that optimal {\lambda} scales linearly with B, for a fixed N,D. However, as N,D scale, we show the optimal timescale obeys a precise power law in the tokens-per-parameter ratio, D/N. This law thus provides a method to accurately predict {\lambda}opt in advance of large-scale training. We also study scaling laws for optimal batch size Bopt (the B enabling lowest loss at a given N,D) and critical batch size Bcrit (the B beyond which further data parallelism becomes ineffective). In contrast with prior work, we find both Bopt and Bcrit scale as power laws in D, independent of model size, N. Finally, we analyze how these findings inform the real-world selection of Pareto-optimal N and D under dual training time and compute objectives.

Cerebras는 Hyperparameter Scaling Law 추정도 시도했군요. 여기에서는 Optimal Timescale = Batch Size / (LR * Weight Decay * Training Data Size)이 Critical Batch Size 이하에서 일정하고 Critical Batch Size는 이전의 연구 결과와 같이 (https://arxiv.org/abs/2503.04715) Training Data Size에만 의존한다는 결론을 냈군요. 흥미롭네요.

<english>
Cerebras also tried to estimate hyperparameter scaling law. The paper insists that optimal timescale = batch size / (LR * weight decay * training data size) is stable under below of the critical batch sizes and critical batch size itself only depends on training data sizes, like previous study (https://arxiv.org/abs/2503.04715). Very interesting.
</english>

#scaling-law #hyperparameter 