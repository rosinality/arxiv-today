https://arxiv.org/abs/2504.05185

*Concise Reasoning via Reinforcement Learning* (Mehdi Fatemi, Banafsheh Rafiee, Mingjie Tang, Kartik Talamadupula)

> Despite significant advancements in large language models (LLMs), a major drawback of reasoning models is their enormous token usage, which increases computational cost, resource requirements, and response time. In this work, we revisit the core principles of reinforcement learning (RL) and, through mathematical analysis, demonstrate that the tendency to generate lengthy responses arises inherently from RL-based optimization during training. This finding questions the prevailing assumption that longer responses inherently improve reasoning accuracy. Instead, we uncover a natural correlation between conciseness and accuracy that has been largely overlooked. Moreover, we show that introducing a secondary phase of RL post-training, using a small set of problems and limited resources, can significantly reduce a model's chain of thought while maintaining or even enhancing accuracy. Finally, we validate our conclusions through extensive experimental results.

PPO를 사용할 때 정답률이 높으면 추론의 길이가 짧아지는 경향이 있다는 분석이군요. VAPO에서도 그렇고 RL 알고리즘의 형태와 길이에 대한 관련성에 대해 좀 더 깊이 분석할 필요가 있네요.

<english>
The analysis suggest that if correct ratio is high then length of reasoning decreases with PPO. Like VAPO we need more deep analysis on relationships between RL algorithms and length.
</english>

#rl #reasoning 