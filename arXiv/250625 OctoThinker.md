https://arxiv.org/abs/2506.20512

*OctoThinker: Mid-training Incentivizes Reinforcement Learning Scaling* (Zengzhi Wang, Fan Zhou, Xuefeng Li, Pengfei Liu)

> Different base language model families, such as Llama and Qwen, exhibit divergent behaviors during post-training with reinforcement learning (RL), especially on reasoning-intensive tasks. What makes a base language model suitable for reinforcement learning? Gaining deeper insight into this question is essential for developing RL-scalable foundation models of the next generation. In this work, we investigate how mid-training strategies shape RL dynamics, focusing on two representative model families: Qwen and Llama. Our study reveals that (1) high-quality mathematical corpora, such as MegaMath-Web-Pro, significantly improve both base model and RL performance, while existing alternatives (e.g., FineMath-4plus) fail to do so; (2) further adding QA-style data, particularly long chain-of-thought (CoT) reasoning examples, enhances RL outcomes, and instruction data further unlocks this effect; (3) while long-CoT improves reasoning depth, it can also induce verbosity of model responses and unstability of RL training, underscoring the importance of data formatting; (4) scaling mid-training consistently leads to stronger downstream RL performance. Building on these insights, we introduce a two-stage mid-training strategy, Stable-then-Decay, in which base models are first trained on 200B tokens with a constant learning rate, followed by 20B tokens across three CoT-focused branches with learning rate decay. This yields OctoThinker, a family of models demonstrating strong RL compatibility and closing the performance gap with more RL-friendly model families, i.e., Qwen. We hope our work will help shape pre-training strategies for foundation models in the RL era. To support further research, we release our open-source models along with a curated math reasoning-intensive corpus of over 70 billion tokens (i.e., MegaMath-Web-Pro-Max).

수학과 Instruction 데이터를 Mid-training에 투입해 추론 RL의 성능을 높인 연구. Mid-training은 중요한 부분이지만 벤치마크를 해킹하기에도 좋은 단계일 것이기 때문에 균형이 필요하겠죠.

<english>
A study that improves reasoning RL by using math and instruction data at mid-training. Mid-training would be crucial stage, but as it would be also useful for hacking the benchmarks, I think we will need to balance it.
</english>

#rl #reasoning #mid-training
