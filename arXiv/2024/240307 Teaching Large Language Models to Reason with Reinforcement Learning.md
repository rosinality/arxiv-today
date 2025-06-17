https://arxiv.org/abs/2403.04642

*Teaching Large Language Models to Reason with Reinforcement Learning* (Alex Havrilla, Yuqing Du, Sharath Chandra Raparthy, Christoforos Nalmpantis, Jane Dwivedi-Yu, Maksym Zhuravinskyi, Eric Hambro, Sainbayar Sukhbaatar, Roberta Raileanu)

> Reinforcement Learning from Human Feedback (\textbf{RLHF}) has emerged as a dominant approach for aligning LLM outputs with human preferences. Inspired by the success of RLHF, we study the performance of multiple algorithms that learn from feedback (Expert Iteration, Proximal Policy Optimization (\textbf{PPO}), Return-Conditioned RL) on improving LLM reasoning capabilities. We investigate both sparse and dense rewards provided to the LLM both heuristically and via a learned reward model. We additionally start from multiple model sizes and initializations both with and without supervised fine-tuning (\textbf{SFT}) data. Overall, we find all algorithms perform comparably, with Expert Iteration performing best in most cases. Surprisingly, we find the sample complexity of Expert Iteration is similar to that of PPO, requiring at most on the order of $10^6$ samples to converge from a pretrained checkpoint. We investigate why this is the case, concluding that during RL training models fail to explore significantly beyond solutions already produced by SFT models. Additionally, we discuss a trade off between maj@1 and pass@96 metric performance during SFT training and how conversely RL training improves both simultaneously. We then conclude by discussing the implications of our findings for RLHF and the future role of RL in LLM fine-tuning.

GSM8K로 RL 실험을 해봤군요. PPO에 더불어 Expert Iteration (Rejection Sampling), Return Conditioning, Outcome Reward Model, 프리트레이닝된 모델에서 시작 vs SFT 모델에서 시작 등에 대해서 비교했습니다.

Expert Iteration이 PPO와 동등한 수준으로 작동한다는 것, 탐색이 많이 발생한다기보다는 학습된 능력을 꺼내오는 패턴으로 학습된다는 것, 그렇지만 RL은 SFT에 비해서 좀 더 다양한 경로로 학습이 가능하고 따라서 일반화 성능이 나을 수 있다는 것 등에 대해 이야기하고 있네요.

#rl 