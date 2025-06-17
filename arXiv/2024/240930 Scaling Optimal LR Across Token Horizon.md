https://arxiv.org/abs/2409.19913

*Scaling Optimal LR Across Token Horizon* (Johan Bjorck, Alon Benhaim, Vishrav Chaudhary, Furu Wei, Xia Song)

> State-of-the-art LLMs are powered by scaling -- scaling model size, dataset size and cluster size. It is economically infeasible to extensively tune hyperparameter for the largest runs. Instead, approximately optimal hyperparameters must be inferred or \textit{transferred} from smaller experiments. Hyperparameter transfer across model sizes has been studied in Yang et al. However, hyperparameter transfer across dataset size -- or token horizon -- has not been studied yet. To remedy this we conduct a large scale empirical study on how optimal learning rate (LR) depends on token horizon in LLM training. We first demonstrate that the optimal LR changes significantly with token horizon -- longer training necessitates smaller LR. Secondly we demonstrate the the optimal LR follows a scaling law, and that the optimal LR for longer horizons can be accurately estimated from shorter horizons via our scaling laws. We also provide a rule-of-thumb for transferring LR across token horizons with zero overhead over current practices. Lastly we provide evidence that LLama-1 used too high LR, and estimate the performance hit from this. We thus argue that hyperparameter transfer across data size is an important and overlooked component of LLM training.

요즘 이야기가 나오는 학습 길이에 따라 LR이 달라져야 하는가에 대한 연구. (https://arxiv.org/abs/2408.13359, https://arxiv.org/abs/2409.15156) 여기서도 학습량이 증가할수록 최적 LR이 좌측으로 이동한다는 것을 발견했네요.

이 문제에 대한 대응 방법은 학습 길이에 따른 최적 LR의 Scaling Law를 추정하는 것. 아이러니하지만 가장 경험적인 규칙인 Scaling Law가 지금은 가장 신뢰로운 도구라는 것을 시사하는 듯 하네요. 이런 형태의 Hyperparameter Scaling Law는 DeepSeek 등에서 시도했었는데 (https://arxiv.org/abs/2401.02954) 꽤 좋은 통찰력이었던 것 같습니다.

<english>
Problem of whether LR should be changed according to training length. (https://arxiv.org/abs/2408.13359, https://arxiv.org/abs/2409.15156) This paper also found that optimal LR left-shifts along with increased duration of the training.

The remedy for this problem is estimating scaling law with respect to training length. Ironically, this suggests that one of the most empirical law, scaling law, is most trustworthy approach for these kind of problems. Previously similar hyperparamter scaling law was tried by DeepSeek. (https://arxiv.org/abs/2401.02954) It seems like that it was quite insightful idea.
</english>

#hyperparameter #scaling-law

# Links

[[240105 DeepSeek LLM.md]]
[[240923 Rethinking Conventional Wisdom in Machine Learning.md]]
[[240823 Power Scheduler.md]]