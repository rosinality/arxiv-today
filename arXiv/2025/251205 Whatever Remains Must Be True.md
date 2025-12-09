https://arxiv.org/abs/2512.05962

*Whatever Remains Must Be True: Filtering Drives Reasoning in LLMs, Shaping Diversity* (Germán Kruszewski, Pierre Erbacher, Jos Rozen, Marc Dymetman)

> Reinforcement Learning (RL) has become the de facto standard for tuning LLMs to solve tasks involving reasoning. However, growing evidence shows that models trained in such way often suffer from a significant loss in diversity. We argue that this arises because RL implicitly optimizes the "mode-seeking" or "zero-forcing" Reverse KL to a target distribution causing the model to concentrate mass on certain high-probability regions of the target while neglecting others. In this work, we instead begin from an explicit target distribution, obtained by filtering out incorrect answers while preserving the relative probabilities of correct ones. Starting from a pre-trained LLM, we approximate this target distribution using the $\alpha$-divergence family, which unifies prior approaches and enables direct control of the precision-diversity trade-off by interpolating between mode-seeking and mass-covering divergences. On a Lean theorem-proving benchmark, our method achieves state-of-the-art performance along the coverage-precision Pareto frontier, outperforming all prior methods on the coverage axis.

다양성 증진을 위한 알파 Divergence (Forward/Reverse KL에 대한 내삽) Distribution Matching. 다만 0/1 Reward를 가정하는 것은 실용적으로 제약이 크다고 생각.

Alpha divergence (which interpolates forward/reverse-KL) distribution matching for better diversity. Though I think solely assuming 0/1 rewards is practically restrictive.

#rl #reasoning 