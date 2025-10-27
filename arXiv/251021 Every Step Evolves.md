https://arxiv.org/abs/2510.18855

*Every Step Evolves: Scaling Reinforcement Learning for Trillion-Scale Thinking Model* (Ling Team)

> We present Ring-1T, the first open-source, state-of-the-art thinking model with a trillion-scale parameter. It features 1 trillion total parameters and activates approximately 50 billion per token. Training such models at a trillion-parameter scale introduces unprecedented challenges, including train-inference misalignment, inefficiencies in rollout processing, and bottlenecks in the RL system. To address these, we pioneer three interconnected innovations: (1) IcePop stabilizes RL training via token-level discrepancy masking and clipping, resolving instability from training-inference mismatches; (2) C3PO++ improves resource utilization for long rollouts under a token budget by dynamically partitioning them, thereby obtaining high time efficiency; and (3) ASystem, a high-performance RL framework designed to overcome the systemic bottlenecks that impede trillion-parameter model training. Ring-1T delivers breakthrough results across critical benchmarks: 93.4 on AIME-2025, 86.72 on HMMT-2025, 2088 on CodeForces, and 55.94 on ARC-AGI-v1. Notably, it attains a silver medal-level result on the IMO-2025, underscoring its exceptional reasoning capabilities. By releasing the complete 1T parameter MoE model to the community, we provide the research community with direct access to cutting-edge reasoning capabilities. This contribution marks a significant milestone in democratizing large-scale reasoning intelligence and establishes a new baseline for open-source model performance.

Ring-1T 테크니컬 리포트. MoE 안정화 (IcePop), 롤아웃 쪼개기 (C3PO++), 비동기 프레임워크의 (ASystem) 조합.

The technical report of Ring-1T. It is **a** combination of stabilization for MoE (IcePop), Rollout partitioning (C3PO++), and asynchronous framework (ASystem).

#rl #framework #reasoning 