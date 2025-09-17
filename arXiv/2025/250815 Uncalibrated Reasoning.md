https://arxiv.org/abs/2508.11800

*Uncalibrated Reasoning: GRPO Induces Overconfidence for Stochastic Outcomes* (Michael Bereket, Jure Leskovec)

> Reinforcement learning (RL) has proven remarkably effective at improving the accuracy of language models in verifiable and deterministic domains like mathematics. Here, we examine if current RL methods are also effective at optimizing language models in verifiable domains with stochastic outcomes, like scientific experiments. Through applications to synthetic data and real-world biological experiments, we demonstrate that Group Relative Policy Optimization (GRPO) induces overconfident probability predictions for binary stochastic outcomes, while Proximal Policy Optimization (PPO) and REINFORCE Leave-One-Out (RLOO) yield well-calibrated models. We show that removing group standard normalization in GRPO fixes its miscalibration and provide a theoretical explanation for why normalization causes overconfidence. Our results provide new evidence against the use of standard normalization in GRPO and help pave the way for applications of RL for reasoning language models beyond deterministic domains.

