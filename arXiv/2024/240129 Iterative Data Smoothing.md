https://arxiv.org/abs/2401.16335

*Iterative Data Smoothing: Mitigating Reward Overfitting and Overoptimization in RLHF* (Banghua Zhu, Michael I. Jordan, Jiantao Jiao)

> Reinforcement Learning from Human Feedback (RLHF) is a pivotal technique that aligns language models closely with human-centric values. The initial phase of RLHF involves learning human values using a reward model from ranking data. It is observed that the performance of the reward model degrades after one epoch of training, and optimizing too much against the learned reward model eventually hinders the true objective. This paper delves into these issues, leveraging the theoretical insights to design improved reward learning algorithm termed 'Iterative Data Smoothing' (IDS). The core idea is that during each training epoch, we not only update the model with the data, but also update the date using the model, replacing hard labels with soft labels. Our empirical findings highlight the superior performance of this approach over the traditional methods.

마이클 조던을 이 문제에 대해서 보게 되네요. Reward Model Overfitting과 그로 인해 이어지는 Overoptimization 문제에 대해 다룹니다. 여기서 보는 주 원인은 Preference 데이터셋의 불균등함과 롱테일적인 특성입니다. 그러니까 많은 비교 데이터가 집중된 사례와 그렇지 않은 사례의 차이에서 발생하는 문제라고 말하고 있네요.

해법으로 제시한 것은 모델의 예측 결과로 레이블을 업데이트해나가는 방법입니다. Secrets of RLHF II의 Label Smoothing이 떠오르는군요. (https://arxiv.org/abs/2401.06080)

#reward-model 

It is interesting to see Michael Jordan in this problem. This paper tackles reward model overfitting problem and overoptimization arose from it. Study suggest that it is the result of imbalancedness and long-tailedness of preference dataset. That is, there are cases that comparison between pair is scarce, in contrast of cases which have enough comparisons. That imbalance causes reward model to overfit.

Solution suggested in this paper is updating ground truth label with model prediction. It reminds me label smoothing from Secrets of RLHF II.

# Links

[[240111 Secrets of RLHF in Large Language Models Part II.md]]