https://arxiv.org/abs/2512.17636

*Trust-Region Adaptive Policy Optimization* (Mingyu Su, Jian Guan, Yuxian Gu, Minlie Huang, Hongning Wang)

> Post-training methods, especially Supervised Fine-Tuning (SFT) and Reinforcement Learning (RL), play an important role in improving large language models' (LLMs) complex reasoning abilities. However, the dominant two-stage pipeline (SFT then RL) suffers from a key inconsistency: SFT enforces rigid imitation that suppresses exploration and induces forgetting, limiting RL's potential for improvements. We address this inefficiency with TRAPO (\textbf{T}rust-\textbf{R}egion \textbf{A}daptive \textbf{P}olicy \textbf{O}ptimization), a hybrid framework that interleaves SFT and RL within each training instance by optimizing SFT loss on expert prefixes and RL loss on the model's own completions, unifying external supervision and self-exploration. To stabilize training, we introduce Trust-Region SFT (TrSFT), which minimizes forward KL divergence inside a trust region but attenuates optimization outside, effectively shifting toward reverse KL and yielding stable, mode-seeking updates favorable for RL. An adaptive prefix-selection mechanism further allocates expert guidance based on measured utility. Experiments on five mathematical reasoning benchmarks show that TRAPO consistently surpasses standard SFT, RL, and SFT-then-RL pipelines, as well as recent state-of-the-art approaches, establishing a strong new paradigm for reasoning-enhanced LLMs.

RL에 SFT를 결합

1. SFT Loss의 Per Token 가중치를 Clipping.

2. 궤적의 리턴에 비례해 Expert에서 가져오는 Prefix의 길이를 조정하고 SFT를 적용. 나머지에 대해서는 RL을 사용.

Incorporating SFT with RL.

1. Clip per-token weight for SFT loss.

2. Relative to the return of the trajectory adjust prefix length from experts and apply SFT to it. For the rest, use RL.

#rl #reasoning 