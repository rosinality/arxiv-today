https://arxiv.org/abs/2504.13818

*Not All Rollouts are Useful: Down-Sampling Rollouts in LLM Reinforcement Learning* (Yixuan Even Xu, Yash Savani, Fei Fang, Zico Kolter)

> Reinforcement learning (RL) has emerged as a powerful paradigm for enhancing reasoning capabilities in large language models, but faces a fundamental asymmetry in computation and memory requirements: inference is embarrassingly parallel with a minimal memory footprint, while policy updates require extensive synchronization and are memory-intensive. To address this asymmetry, we introduce PODS (Policy Optimization with Down-Sampling), a framework that strategically decouples these phases by generating numerous rollouts in parallel but updating only on an informative subset. Within this framework, we develop max-variance down-sampling, a theoretically motivated method that selects rollouts with maximally diverse reward signals. We prove that this approach has an efficient algorithmic solution, and empirically demonstrate that GRPO with PODS using max-variance down-sampling achieves superior performance over standard GRPO on the GSM8K benchmark.

RL 과정의 샘플링의 규모를 늘리고 그 중에서 Reward의 분산을 최대화 하는 샘플들을 선택한다는 아이디어.

<english>
The idea of increase number of samples during RL and downsamples it by choosing samples that maximizes variance.
</english>

#rl 