https://arxiv.org/abs/2510.07284

*Online Rubrics Elicitation from Pairwise Comparisons* (MohammadHossein Rezaei, Robert Vacareanu, Zihao Wang, Clinton Wang, Yunzhong He, Afra Feyza Akyürek)

> Rubrics provide a flexible way to train LLMs on open-ended long-form answers where verifiable rewards are not applicable and human preferences provide coarse signals. Prior work shows that reinforcement learning with rubric-based rewards leads to consistent gains in LLM post-training. Most existing approaches rely on rubrics that remain static over the course of training. Such static rubrics, however, are vulnerable to reward-hacking type behaviors and fail to capture emergent desiderata that arise during training. We introduce Online Rubrics Elicitation (OnlineRubrics), a method that dynamically curates evaluation criteria in an online manner through pairwise comparisons of responses from current and reference policies. This online process enables continuous identification and mitigation of errors as training proceeds. Empirically, this approach yields consistent improvements of up to 8% over training exclusively with static rubrics across AlpacaEval, GPQA, ArenaHard as well as the validation sets of expert questions and rubrics. We qualitatively analyze the elicited criteria and identify prominent themes such as transparency, practicality, organization, and reasoning.

모델의 거동의 변화와 Reward Hacking에 대응하기 위해 루브릭을 모델의 학습 과정과 함께 생성. LLM이 현재 필요한 루브릭이 무엇인지 정확히 판단하도록 통제하는 것이 아무래도 까다로운 문제일 듯.

Generating rubrics alongside model training to address changes in model behavior and reward hacking. Controlling how LLMs determine which rubrics are currently needed would likely be a hard problem.

#rl 