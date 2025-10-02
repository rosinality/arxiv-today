https://arxiv.org/abs/2509.25808

*Improving Sampling Efficiency in RLVR through Adaptive Rollout and Response Reuse* (Yuheng Zhang, Wenlin Yao, Changlong Yu, Yao Liu, Qingyu Yin, Bing Yin, Hyokun Yun, Lihong Li)

> Large language models (LLMs) have achieved impressive reasoning performance, with reinforcement learning with verifiable rewards (RLVR) emerging as a standard paradigm for post-training. A representative algorithm, group relative policy optimization (GRPO) (Shao et al., 2024), computes advantages by normalizing outcome rewards within response groups, but suffers from a vanishing advantage issue when all responses in a group receive identical rewards. To address this issue, we propose Adaptive Rollout and Response Reuse Policy Optimization (AR3PO), a sampling efficient RLVR algorithm that introduces two novel techniques: adaptive rollout, which dynamically allocates more responses to difficult prompts while saving computation on easier ones, and response reuse, which leverages previously generated correct responses to provide useful training signals. We compare AR3PO with strong RLVR baselines on multiple representative benchmarks using two different families of base models. Across the 7B and 8B models, AR3PO consistently outperforms GRPO and matches or surpasses DAPO (Yu et al., 2025), reducing rollout cost by up to 4.2x. On the larger 32B model, AR3PO achieves comparable performance to DAPO at similar training steps while maintaining substantially lower rollout cost.

샘플 효율성 향상. 최소한 하나의 응답이 정답일 때까지만 응답 그룹을 샘플링. 리플레이 버퍼 사용.

Enhancing sampling efficiency. Adaptively sample groups of responses until at least one of them is correct. Use a replay buffer.

#rl #reasoning 