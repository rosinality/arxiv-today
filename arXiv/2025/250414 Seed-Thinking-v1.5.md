https://github.com/ByteDance-Seed/Seed-Thinking-v1.5/blob/main/seed-thinking-v1.5.pdf

*Seed-Thinking-v1.5: Advancing Superb Reasoning Models with Reinforcement Learning* (ByteDance Seed)

> We introduce Seed-Thinking-v1.5, capable of reasoning through thinking before responding, resulting in improved performance on a wide range of benchmarks. Seed-Thinking-v1.5 achieves 86.7 on AIME 2024, 55.0 on Codeforces and 77.3 on GPQA, demonstrating excellent reasoning abilities in STEM and coding. Beyond reasoning tasks, the method demonstrates notable generalization across diverse domains. For instance, it surpasses DeepSeek R1 by 8% in win rate on non-reasoning tasks, indicating its broader applicability. Compared to other state-of-the-art reasoning models, Seed-Thinking-v1.5 is a Mixture-of-Experts (MoE) model with a relatively small size, featuring 20B activated and 200B total parameters. As part of our effort to assess generalized reasoning, we develop two internal benchmarks, BeyondAIME and Codeforces, both of which will be publicly released to support future research.

ByteDance의 추론 모델. 규칙 및 휴리스틱 기반이 아니라 Reference Answer를 입력으로 받아 추론을 통해 검증하는 검증 모델을 사용했네요. 그리고 VAPO를 썼군요 (https://arxiv.org/abs/2504.05118).

<english>
Reasoning model from ByteDance. Instead of rule and heuristic based verifier, they used verifier model that uses reference answer input and doing a verification through reasoning. And they employed VAPO (https://arxiv.org/abs/2504.05118).
</english>

#reasoning #rl #rlhf 