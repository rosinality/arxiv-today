https://arxiv.org/abs/2511.19942

*Differential Smoothing Mitigates Sharpening and Improves LLM Reasoning* (Jingchu Gai, Guanning Zeng, Huaqing Zhang, Aditi Raghunathan)

> It is widely recognized that reinforcement learning (RL) fine-tuning of large language models often leads to \textit{diversity collapse}, where outputs lack variety. Prior work has proposed a range of heuristics to counteract this effect, but these methods are ad hoc: they frequently trade off correctness for diversity, their effectiveness varies across tasks, and in some cases they even contradict one another. In this work, we place these observations on a rigorous foundation. We first provide a formal proof of why RL fine-tuning exhibits diversity collapse via a selection and reinforcement bias. Next, we make a key observation that any reward modification to address diversity collapse only needs to be applied on the correct trajectories. Building directly on this analysis, we introduce a principled method -- \textit{differential smoothing} -- that provably improves both correctness and diversity, outperforming vanilla RL as well as widely used entropy-based heuristics. Our theory precisely characterizes when existing heuristics help and why they fail, while showing that differential smoothing is universally superior. Extensive experiments with models from 1B to 7B parameters, across domains including CountDown and real-world mathematical reasoning, demonstrate consistent gains. Differential smoothing improves both Pass@1 and Pass@k, with up to 6.7\% improvements on AIME24 dataset.

정답에 대해 엔트로피 보너스, 오답에 대해서는 엔트로피 페널티를 가해 정답률과 다양성을 동시에 촉진. 가끔 엔트로피가 탐색을 촉진하기 위해 제어 대상이 되는 경우가 있음. 그러나 좀 더 섬세한 척도가 필요할지도.

Entropy bonus for positives and penalty for negatives to enhance both correctness and diversity. Sometimes entropy itself is the target of control to enhance exploration. But maybe more sophisticated measures are needed?

#rl 