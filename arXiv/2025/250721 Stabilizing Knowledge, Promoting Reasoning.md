https://arxiv.org/abs/2507.15778

*Stabilizing Knowledge, Promoting Reasoning: Dual-Token Constraints for RLVR* (Jiakang Wang, Runze Liu, Fuzheng Zhang, Xiu Li, Guorui Zhou)

> Reinforcement Learning with Verifiable Rewards (RLVR) has become an effective post-training method for improving the reasoning abilities of Large Language Models (LLMs), mainly by shaping higher-order behaviors such as reflection and planning. However, previous RLVR algorithms often apply uniform training signals to all tokens, without considering the different roles of low-entropy knowledge-related tokens and high-entropy reasoning-related tokens. Some recent methods try to separate these token types by gradient masking or asynchronous updates, but these approaches may break semantic dependencies in the model output and hinder effective learning. In this work, we propose Archer, an entropy-aware RLVR approach with dual-token constraints and synchronous updates. Specifically, our method applies weaker KL regularization and higher clipping thresholds to reasoning tokens to encourage exploration, while using stronger constraints on knowledge tokens to maintain factual knowledge. Experimental results on several mathematical reasoning and code generation benchmarks show that our approach significantly outperforms previous RLVR methods, reaching or exceeding state-of-the-art performance among models of comparable size. The code is available at https://github.com/wizard-III/ArcherCodeR.

이젠 아예 엔트로피가 높은 토큰을 추론 토큰, 낮은 토큰을 지식 토큰으로 분류하기 시작. 엔트로피가 낮은 토큰을 학습에서 아예 배제하는 것은 부적절하니 Clipping과 KL을 조절한다는 아이디어.

Now high-entropy tokens become reasoning tokens and low-entropy tokens are considered as knowledge tokens. Excluding low-entropy tokens from training would be excessive, thus adjust clipping and KL per entropy.

#rl #reasoning 