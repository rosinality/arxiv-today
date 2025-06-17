https://arxiv.org/abs/2506.02177

*Act Only When It Pays: Efficient Reinforcement Learning for LLM Reasoning via Selective Rollouts* (Haizhong Zheng, Yang Zhou, Brian R. Bartoldson, Bhavya Kailkhura, Fan Lai, Jiawei Zhao, Beidi Chen)

> Reinforcement learning, such as PPO and GRPO, has powered recent breakthroughs in LLM reasoning. Scaling rollout to sample more prompts enables models to selectively use higher-quality data for training, which can stabilize RL training and improve model performance. However, this comes at the cost of significant computational overhead. In this paper, we show that a substantial portion of this overhead can be avoided by skipping uninformative prompts before rollout. Our analysis of reward dynamics reveals a strong temporal consistency in prompt value: prompts that are uninformative in one epoch of training are likely to remain uninformative in future epochs. Based on these insights, we propose GRESO (GRPO with Efficient Selective Rollout), an online, lightweight pre-rollout filtering algorithm that predicts and skips uninformative prompts using reward training dynamics. By evaluating GRESO on a broad range of math reasoning benchmarks and models, such as Qwen2.5-Math-1.5B, DeepSeek-R1-Distill-Qwen-1.5B, and Qwen2.5-Math-7B, we show that GRESO achieves up to 2.4x wall-clock time speedup in rollout and up to 2.0x speedup in total training time without accuracy degradation.

Reward 분산이 한 번 0이었던 프롬프트는 이후에도 그럴 가능성이 높으니 걸러낸다는 아이디어. 그렇지만 이후 패턴이 달라질 수도 있으니 일정 확률로 다시 사용합니다.

<english>
The idea of filter out prompt with 0 reward variances, as it is probable to like that thereafter. But as it is possible to change in patterns later, it reuses that at certain probabilities.
</english>

#rl #reasoning 