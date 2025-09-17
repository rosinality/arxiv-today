https://arxiv.org/abs/2509.04259

*RL's Razor: Why Online Reinforcement Learning Forgets Less* (Idan Shenfeld, Jyothish Pari, Pulkit Agrawal)

> Comparison of fine-tuning models with reinforcement learning (RL) and supervised fine-tuning (SFT) reveals that, despite similar performance at a new task, RL preserves prior knowledge and capabilities significantly better. We find that the degree of forgetting is determined by the distributional shift, measured as the KL-divergence between the fine-tuned and base policy evaluated on the new task. Our analysis reveals that on-policy RL is implicitly biased towards KL-minimal solutions among the many that solve the new task, whereas SFT can converge to distributions arbitrarily far from the base model. We validate these findings through experiments with large language models and robotic foundation models and further provide theoretical justification for why on-policy RL updates lead to a smaller KL change. We term this principle $\textit{RL's Razor}$: among all ways to solve a new task, RL prefers those closest in KL to the original model.

RL이 베이스 모델로부터 KL-최소 솔루션에 도달하기에 OOD에 대한 성능이 유지된다는 주장.

The author insists that RL reaches a KL-minimal solution from the base model, thus keeping the performance on OOD tasks.

#rl #generalization 