https://arxiv.org/abs/2411.00750

*Mitigating Tail Narrowing in LLM Self-Improvement via Socratic-Guided Sampling* (Yiwen Ding, Zhiheng Xi, Wei He, Zhuoyuan Li, Yitao Zhai, Xiaowei Shi, Xunliang Cai, Tao Gui, Qi Zhang, Xuanjing Huang)

> Self-improvement methods enable large language models (LLMs) to generate solutions themselves and iteratively train on filtered, high-quality rationales. This process proves effective and reduces the reliance on human supervision in LLMs' reasoning, but the performance soon plateaus. We delve into the process and find that models tend to over-sample on easy queries and under-sample on queries they have yet to master. As iterations proceed, this imbalance in sampling is exacerbated, leading to a long-tail distribution where solutions to difficult queries almost diminish. This phenomenon limits the performance gain of self-improving models. A straightforward solution is brute-force sampling to balance the distribution, which significantly raises computational costs. In this paper, we introduce Guided Self-Improvement (GSI), a strategy aimed at improving the efficiency of sampling challenging heavy-tailed data. It leverages Socratic-style guidance signals to help LLM reasoning with complex queries, reducing the exploration effort and minimizing computational overhead. Experiments on four models across diverse mathematical tasks show that GSI strikes a balance between performance and efficiency, while also being effective on held-out tasks.

모델에서 샘플링을 한 다음 정답인 샘플들만 필터링해서 학습한다면 정답일 확률이 높은 쉬운 데이터로 학습 데이터가 편향될 가능성이 높겠죠. 샘플링-필터링을 사용하는 방법에서는 중요한 문제일 듯 하네요. 해결 방법으로 제시한 것은 난이도가 높은 샘플에 대한 성공 확률을 높이기 위해 Privileged Information을 사용하는 방법들입니다.

<english>
If we train the model with samples from the model, and filter which answer is correct, then training data will be biased towards easier samples that probability of correct is high. I think this is important problem for the methods which uses sampling and filtering. Solution for this problem is increasing probability of correct by incorporating privileged informations.
</english>

#synthetic-data 