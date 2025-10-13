https://arxiv.org/abs/2510.08141

*Arbitrary Entropy Policy Optimization: Entropy Is Controllable in Reinforcement Finetuning* (Chen Wang, Zhaochun Li, Jionghao Bai, Yuzhi Zhang, Shisheng Cui, Zhou Zhao, Yue Wang)

> Reinforcement finetuning (RFT) is essential for enhancing the reasoning capabilities of large language models (LLM), yet the widely adopted Group Relative Policy Optimization (GRPO) suffers from entropy collapse, where entropy monotonically decreases, exploration vanishes, and policies converge prematurely. Existing entropy-regularized methods only partially alleviate this issue while introducing bias and instability, leaving entropy control unresolved and the connection between entropy, exploration, and performance unclear. We propose Arbitrary Entropy Policy Optimization (AEPO), which eliminates entropy collapse by replacing entropy bonuses with REINFORCE policy gradient on temperature-adjusted distributions and stabilizing entropy through temperature regulation. AEPO integrates three key designs: policy gradient as regularization, distribution as regularization, and REINFORCE as regularization, enabling precise entropy control without distorting optimization. Experiments demonstrate three major contributions: AEPO (1) stabilizes entropy at arbitrary target levels, effectively removing collapse in GRPO; (2) reveals a non-monotonic relation where performance first improves then declines with increasing entropy, clarifying the link between entropy, exploration, and reasoning; and (3) generalizes beyond entropy, providing a broader RFT paradigm where superior target distributions can serve as REINFORCE regularizers.

Temperature를 조정한 샘플을 사용해 계산한 REINFORCE Loss를 Regularizer로 사용해 엔트로피의 거동을 통제.

Control entropy dynamics using REINFORCE loss computed from temperature-adjusted samples as regularization.

#rl #reasoning 