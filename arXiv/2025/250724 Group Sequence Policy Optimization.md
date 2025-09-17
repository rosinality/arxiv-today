https://arxiv.org/abs/2507.18071

*Group Sequence Policy Optimization* (Chujie Zheng, Shixuan Liu, Mingze Li, Xiong-Hui Chen, Bowen Yu, Chang Gao, Kai Dang, Yuqiong Liu, Rui Men, An Yang, Jingren Zhou, Junyang Lin)

> This paper introduces Group Sequence Policy Optimization (GSPO), our stable, efficient, and performant reinforcement learning algorithm for training large language models. Unlike previous algorithms that adopt token-level importance ratios, GSPO defines the importance ratio based on sequence likelihood and performs sequence-level clipping, rewarding, and optimization. We demonstrate that GSPO achieves superior training efficiency and performance compared to the GRPO algorithm, notably stabilizes Mixture-of-Experts (MoE) RL training, and has the potential for simplifying the design of RL infrastructure. These merits of GSPO have contributed to the remarkable improvements in the latest Qwen3 models.

GRPO를 시퀀스 레벨 Objective로 수정. 토큰 단위냐 시퀀스 단위냐는 고전적인 주제. MoE에 대해 더 안정적이고 Likelihood 재계산이 필요하지 않다 같은 실용적인 장점을 주장.

Sequence level GRPO. The token vs sequence-level objective is a classical topic Claims practical advantages such as stability for MoE and removal of likelihood recomputation.

#rl #reasoning 