https://arxiv.org/abs/2509.09177

*Clip Your Sequences Fairly: Enforcing Length Fairness for Sequence-Level RL* (Hanyi Mao, Quanjia Xiao, Lei Pang, Haixiao Liu)

> We propose FSPO (Fair Sequence Policy Optimization), a sequence-level reinforcement learning method for LLMs that enforces length-fair clipping directly in the importance-sampling (IS) weight space. We revisit sequence-level RL methods and identify a mismatch when PPO/GRPO-style clipping is transplanted to sequences: a fixed clip range systematically reweights short vs. long responses, distorting the effective objective. Theoretically, we formalize length fairness via a Length Reweighting Error (LRE) and prove that small LRE yields a directional cosine guarantee between the clipped and true updates. FSPO introduces a simple, Gaussian-motivated remedy: we clip the sequence log-IS ratio with a band that applies a KL-corrected drift term and scales as $\sqrt{L}$. Empirically, FSPO flattens clip rates across length bins, stabilizes training, and outperforms all baselines across multiple evaluation datasets.

시퀀스 레벨 Importance Weighting을 사용한다면 클리핑 확률은 길이와 관계 없이 일정해야 하지 않겠는가 하는 아이디어. 아직 드래프트.

The idea that if we use sequence-level importance weighting, then the probability of clipping should be constant regardless of length. Work in progress.

#rl 