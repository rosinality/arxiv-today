https://arxiv.org/abs/2505.18830

*On the Effect of Negative Gradient in Group Relative Deep Reinforcement Optimization* (Wenlong Deng, Yi Ren, Muchen Li, Danica J. Sutherland, Xiaoxiao Li, Christos Thrampoulidis)

> Reinforcement learning (RL) has become popular in enhancing the reasoning capabilities of large language models (LLMs), with Group Relative Policy Optimization (GRPO) emerging as a widely used algorithm in recent systems. Despite GRPO's widespread adoption, we identify a previously unrecognized phenomenon we term Lazy Likelihood Displacement (LLD), wherein the likelihood of correct responses marginally increases or even decreases during training. This behavior mirrors a recently discovered misalignment issue in Direct Preference Optimization (DPO), attributed to the influence of negative gradients. We provide a theoretical analysis of GRPO's learning dynamic, identifying the source of LLD as the naive penalization of all tokens in incorrect responses with the same strength. To address this, we develop a method called NTHR, which downweights penalties on tokens contributing to the LLD. Unlike prior DPO-based approaches, NTHR takes advantage of GRPO's group-based structure, using correct responses as anchors to identify influential tokens. Experiments on math reasoning benchmarks demonstrate that NTHR effectively mitigates LLD, yielding consistent performance gains across models ranging from 0.5B to 3B parameters.

GRPO에서 정답 시퀀스의 확률도 낮아지는 현상에 대한 분석. 모든 토큰을 Negative로 처리하는 것이 문제이고 따라서 토큰 단위 Reward를 주어야 한다고.

<english>
Analysis on the phenomenon of decreasing probability of correct sequences in GRPO. The main problem lies in considering all tokens as a negative unifomly, thus we need token level rewards.
</english>

#rl #reasoning 