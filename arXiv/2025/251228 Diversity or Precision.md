https://arxiv.org/abs/2512.22955

*Diversity or Precision? A Deep Dive into Next Token Prediction* (Haoyuan Wu, Hai Wang, Jiajia Wu, Jinxiang Ou, Keyao Wang, Weile Chen, Zihao Zheng, Bei Yu)

> Recent advancements have shown that reinforcement learning (RL) can substantially improve the reasoning abilities of large language models (LLMs). The effectiveness of such RL training, however, depends critically on the exploration space defined by the pre-trained model's token-output distribution. In this paper, we revisit the standard cross-entropy loss, interpreting it as a specific instance of policy gradient optimization applied within a single-step episode. To systematically study how the pre-trained distribution shapes the exploration potential for subsequent RL, we propose a generalized pre-training objective that adapts on-policy RL principles to supervised learning. By framing next-token prediction as a stochastic decision process, we introduce a reward-shaping strategy that explicitly balances diversity and precision. Our method employs a positive reward scaling factor to control probability concentration on ground-truth tokens and a rank-aware mechanism that treats high-ranking and low-ranking negative tokens asymmetrically. This allows us to reshape the pre-trained token-output distribution and investigate how to provide a more favorable exploration space for RL, ultimately enhancing end-to-end reasoning performance. Contrary to the intuition that higher distribution entropy facilitates effective exploration, we find that imposing a precision-oriented prior yields a superior exploration space for RL.

Cross Entropy의 암시적인 Reward에 대해 Reward Shaping을 적용해 프리트레이닝 시점에서 Diversity와 Precision 사이의 균형을 조정.

Adjusting the balance of diversity and precision in pretraining by applying reward shaping on the implicit reward of cross entropy.

#pretraining 