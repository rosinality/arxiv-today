https://arxiv.org/abs/2512.18160

*Propose, Solve, Verify: Self-Play Through Formal Verification* (Alex Wilf, Pranjal Aggarwal, Bryan Parno, Daniel Fried, Louis-Philippe Morency, Paul Pu Liang, Sean Welleck)

> Training models through self-play alone (without any human data) has been a longstanding goal in AI, but its effectiveness for training large language models remains unclear, particularly in code generation where rewards based on unit tests are brittle and prone to error propagation. We study self-play in the verified code generation setting, where formal verification provides reliable correctness signals. We introduce Propose, Solve, Verify (PSV) a simple self-play framework where formal verification signals are used to create a proposer capable of generating challenging synthetic problems and a solver trained via expert iteration. We use PSV to train PSV-Verus, which across three benchmarks improves pass@1 by up to 9.6x over inference-only and expert-iteration baselines. We show that performance scales with the number of generated questions and training iterations, and through ablations identify formal verification and difficulty-aware proposal as essential ingredients for successful self-play.

Formal Verification으로 Reward를 부여하는 코딩 Self-play RL. Formal Verification이 실용적인 문제들에 대해 광범위하게 적용 가능할지? (잘 모르는 주제.)

Self-play RL for coding with formal verification to assign the reward. Would formal verification be widely applicable to practical problems? (I don't know much about this.)

#rl 