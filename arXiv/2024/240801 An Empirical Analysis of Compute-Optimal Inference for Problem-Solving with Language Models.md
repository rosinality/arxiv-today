https://arxiv.org/abs/2408.00724

*An Empirical Analysis of Compute-Optimal Inference for Problem-Solving with Language Models* (Yangzhen Wu, Zhiqing Sun, Shanda Li, Sean Welleck, Yiming Yang)

> The optimal training configurations of large language models (LLMs) with respect to model sizes and compute budgets have been extensively studied. But how to optimally configure LLMs during inference has not been explored in sufficient depth. We study compute-optimal inference: designing models and inference strategies that optimally trade off additional inference-time compute for improved performance. As a first step towards understanding and designing compute-optimal inference methods, we assessed the effectiveness and computational efficiency of multiple inference strategies such as Greedy Search, Majority Voting, Best-of-N, Weighted Voting, and their variants on two different Tree Search algorithms, involving different model sizes and computational budgets. We found that a smaller language model with a novel tree search algorithm typically achieves a Pareto-optimal trade-off. These results highlight the potential benefits of deploying smaller models equipped with more sophisticated decoding algorithms in budget-constrained scenarios, e.g., on end-devices, to enhance problem-solving accuracy. For instance, we show that the Llemma-7B model can achieve competitive accuracy to a Llemma-34B model on MATH500 while using $2\times$ less FLOPs. Our findings could potentially apply to any generation task with a well-defined measure of success.

추론 시 사용 연산량에 따른 성능 변화에 대한 Scaling Law. 얼마 전 나온 논문과 비슷하고 (https://arxiv.org/abs/2407.21787) 이쪽에서도 (Reward Model을 사용했기에 더더욱) 꺾이는 지점이 나타나는 듯 합니다. 다만 서치 알고리즘에 따라 이 점근선을 이동시킬 수 있겠다는 생각도 들긴 하네요.

#search #scaling-law

# Links

[[240731 Large Language Monkeys.md]]