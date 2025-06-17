https://arxiv.org/abs/2404.01067

*Exploring the Mystery of Influential Data for Mathematical Reasoning* (Xinzhe Ni, Yeyun Gong, Zhibin Gou, Yelong Shen, Yujiu Yang, Nan Duan, Weizhu Chen)

> Selecting influential data for fine-tuning on downstream tasks is a key factor for both performance and computation efficiency. Recent works have shown that training with only limited data can show a superior performance on general tasks. However, the feasibility on mathematical reasoning tasks has not been validated. To go further, there exist two open questions for mathematical reasoning: how to select influential data and what is an influential data composition. For the former one, we propose a Quality-aware Diverse Selection (QaDS) strategy adaptable for mathematical reasoning. A comparison with other selection strategies validates the superiority of QaDS. For the latter one, we first enlarge our setting and explore the influential data composition. We conduct a series of experiments and highlight: scaling up reasoning data, and training with general data selected by QaDS is helpful. Then, we define our optimal mixture as OpenMathMix, an influential data mixture with open-source data selected by QaDS. With OpenMathMix, we achieve a state-of-the-art 48.8% accuracy on MATH with 7B base model. Additionally, we showcase the use of QaDS in creating efficient fine-tuning mixtures with various selection ratios, and analyze the quality of a wide range of open-source datasets, which can perform as a reference for future works on mathematical reasoning tasks.

Diversity-Quality 필터링의 한 사례. 수학 Instruction 데이터에 대해서 했군요. Diversity는 임베딩 Coreset Sampling을 썼고 Quality에 대해서는 1-shot으로 줬을 때의 확률 변화를 사용했군요. (https://arxiv.org/abs/2312.10302) 1-shot 스코어가 얼마나 괜찮은지 불확실성이 있긴 하지만 여튼 기본적으로 생각해볼 수 있는 세팅일 것 같습니다.

#dataset

# Links

[[231216 One Shot Learning as Instruction Data Prospector for Large Language Models.md]]