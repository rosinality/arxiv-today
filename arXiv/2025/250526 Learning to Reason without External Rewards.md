https://arxiv.org/abs/2505.19590

*Learning to Reason without External Rewards* (Xuandong Zhao, Zhewei Kang, Aosong Feng, Sergey Levine, Dawn Song)

> Training large language models (LLMs) for complex reasoning via Reinforcement Learning with Verifiable Rewards (RLVR) is effective but limited by reliance on costly, domain-specific supervision. We explore Reinforcement Learning from Internal Feedback (RLIF), a framework that enables LLMs to learn from intrinsic signals without external rewards or labeled data. We propose Intuitor, an RLIF method that uses a model's own confidence, termed self-certainty, as its sole reward signal. Intuitor replaces external rewards in Group Relative Policy Optimization (GRPO) with self-certainty scores, enabling fully unsupervised learning. Experiments demonstrate that Intuitor matches GRPO's performance on mathematical benchmarks while achieving superior generalization to out-of-domain tasks like code generation, without requiring gold solutions or test cases. Our findings show that intrinsic model signals can drive effective learning across domains, offering a scalable alternative to RLVR for autonomous AI systems where verifiable rewards are unavailable. Code is available at https://github.com/sunblaze-ucb/Intuitor

모델의 Certainty 기반으로 Verifier 없이 추론 RL (https://arxiv.org/abs/2504.05812). RL로 모델에 새로운 능력을 주입할 수 있는가라는 논쟁에 더해 데이터 없이 성능을 향상시키는 시도가 계속 나오겠죠. 좋은 방향일까요.

<english>
Reasoning RL without verifiers based on model's certainty on the outputs (https://arxiv.org/abs/2504.05812). In addition to whether it is possible RL to inject new capabilities into the model, there would be continuous attempt to improve the performance without the data. Would it be good direction?
</english>

#rl #reasoning 