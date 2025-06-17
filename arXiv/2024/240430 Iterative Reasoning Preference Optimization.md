https://arxiv.org/abs/2404.19733

*Iterative Reasoning Preference Optimization* (Richard Yuanzhe Pang, Weizhe Yuan, Kyunghyun Cho, He He, Sainbayar Sukhbaatar, Jason Weston)

> Iterative preference optimization methods have recently been shown to perform well for general instruction tuning tasks, but typically make little improvement on reasoning tasks (Yuan et al., 2024, Chen et al., 2024). In this work we develop an iterative approach that optimizes the preference between competing generated Chain-of-Thought (CoT) candidates by optimizing for winning vs. losing reasoning steps that lead to the correct answer. We train using a modified DPO loss (Rafailov et al., 2023) with an additional negative log-likelihood term, which we find to be crucial. We show reasoning improves across repeated iterations of this scheme. While only relying on examples in the training set, our approach results in increasing accuracy for Llama-2-70B-Chat from 55.6% to 81.6% on GSM8K (and 88.7% with majority voting out of 32 samples), from 12.5% to 20.8% on MATH, and from 77.8% to 86.7% on ARC-Challenge, which outperforms other Llama-2-based models not relying on additionally sourced datasets.

문제에 대해 Chain of Thought Rationale을 생성하고 정답이 맞은 경우를 Positive, 맞지 않은 경우를 Negative로 해서 DPO Loss와 Positive에 대한 NLL Loss로 학습시킵니다. 그리고 이렇게 학습한 모델로 Chain of Thought 생성부터 다시 반복하네요.

답이 주어진다면 많은 것을 할 수 있다는 사례가 하나 더 추가됐네요. 이제 답을 어떻게 찾아낼 것인가가 점점 더 문제가 될 듯 합니다.

#self-improvement 