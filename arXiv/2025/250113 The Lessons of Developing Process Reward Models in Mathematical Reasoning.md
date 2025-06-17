https://arxiv.org/abs/2501.07301

*The Lessons of Developing Process Reward Models in Mathematical Reasoning* (Zhenru Zhang, Chujie Zheng, Yangzhen Wu, Beichen Zhang, Runji Lin, Bowen Yu, Dayiheng Liu, Jingren Zhou, Junyang Lin)

> Process Reward Models (PRMs) emerge as a promising approach for process supervision in mathematical reasoning of Large Language Models (LLMs), which aim to identify and mitigate intermediate errors in the reasoning processes. However, the development of effective PRMs faces significant challenges, particularly in data annotation and evaluation methodologies. In this paper, through extensive experiments, we demonstrate that commonly used Monte Carlo (MC) estimation-based data synthesis for PRMs typically yields inferior performance and generalization compared to LLM-as-a-judge and human annotation methods. MC estimation relies on completion models to evaluate current-step correctness, leading to inaccurate step verification. Furthermore, we identify potential biases in conventional Best-of-N (BoN) evaluation strategies for PRMs: (1) The unreliable policy models generate responses with correct answers but flawed processes, leading to a misalignment between the evaluation criteria of BoN and the PRM objectives of process verification. (2) The tolerance of PRMs of such responses leads to inflated BoN scores. (3) Existing PRMs have a significant proportion of minimum scores concentrated on the final answer steps, revealing the shift from process to outcome-based assessment in BoN Optimized PRMs. To address these challenges, we develop a consensus filtering mechanism that effectively integrates MC estimation with LLM-as-a-judge and advocates a more comprehensive evaluation framework that combines response-level and step-level metrics. Based on the mechanisms, we significantly improve both model performance and data efficiency in the BoN evaluation and the step-wise error identification task. Finally, we release a new state-of-the-art PRM that outperforms existing open-source alternatives and provides practical guidelines for future research in building process supervision models.

Process Reward Model에 대한 분석. 정답 여부로 과정에 대한 평가를 학습한 모델들은 (MC) PRM에 대한 벤치마크 점수에 비해 (https://arxiv.org/abs/2412.06559) BoN 평가의 점수가 부풀려지는 경향이 있다고. 이는 과정에 대한 평가가 정확하지 않기 때문입니다.

이에 대해서는 LLM Critic이 오히려 정확했다고 하네요. 그래서 LLM Critic으로 추가 필터링 하는 시도를 했습니다.

<english>
Analysis on process reward model. Models trained by evaluating processes by final correctness (MC) has tendency to have overestimated score of BoN evaluation compared to benchmark for PRM (https://arxiv.org/abs/2412.06559). It is because of inaccuracies of evaluating processes

For this respect LLM critic was more accurate. So they tried to further filter samples using LLM critic.
</english>

#reward-model

# Links

[[241209 ProcessBench.md]]