https://arxiv.org/abs/2509.04575

*Bootstrapping Task Spaces for Self-Improvement* (Minqi Jiang, Andrei Lupu, Yoram Bachrach)

> Progress in many task domains emerges from repeated revisions to previous solution attempts. Training agents that can reliably self-improve over such sequences at inference-time is a natural target for reinforcement learning (RL), yet the naive approach assumes a fixed maximum iteration depth, which can be both costly and arbitrary. We present Exploratory Iteration (ExIt), a family of autocurriculum RL methods that directly exploits the recurrent structure of self-improvement tasks to train LLMs to perform multi-step self-improvement at inference-time while only training on the most informative single-step iterations. ExIt grows a task space by selectively sampling the most informative intermediate, partial histories encountered during an episode for continued iteration, treating these starting points as new self-iteration task instances to train a self-improvement policy. ExIt can further pair with explicit exploration mechanisms to sustain greater task diversity. Across several domains, encompassing competition math, multi-turn tool-use, and machine learning engineering, we demonstrate that ExIt strategies, starting from either a single or many task instances, can produce policies exhibiting strong inference-time self-improvement on held-out task instances, and the ability to iterate towards higher performance over a step budget extending beyond the average iteration depth encountered during training.

단일 턴 개선만으로 학습해서 자신의 응답을 K번 개선할 수 있는 모델 학습. K 턴에 대한 샘플을 버퍼에서 샘플링한 다음 Policy에게 K+1 턴에 해당하는 응답 개선을 수행하도록 함.

Training a model to improve its own responses K times using single-turn improvements only. This is done by sampling K turn samples from the buffer and letting the policy improve them to generate K+1 turn samples.

#rl #self-improvement 