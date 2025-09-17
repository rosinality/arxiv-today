https://arxiv.org/abs/2509.07558

*$ΔL$ Normalization: Rethink Loss Aggregation in RLVR* (Zhiyuan He, Xufang Luo, Yike Zhang, Yuqing Yang, Lili Qiu)

> We propose $\Delta L$ Normalization, a simple yet effective loss aggregation method tailored to the characteristic of dynamic generation lengths in Reinforcement Learning with Verifiable Rewards (RLVR). Recently, RLVR has demonstrated strong potential in improving the reasoning capabilities of large language models (LLMs), but a major challenge lies in the large variability of response lengths during training, which leads to high gradient variance and unstable optimization. Although previous methods such as GRPO, DAPO, and Dr. GRPO introduce different loss normalization terms to address this issue, they either produce biased estimates or still suffer from high gradient variance. By analyzing the effect of varying lengths on policy loss both theoretically and empirically, we reformulate the problem as finding a minimum-variance unbiased estimator. Our proposed $\Delta L$ Normalization not only provides an unbiased estimate of the true policy loss but also minimizes gradient variance in theory. Extensive experiments show that it consistently achieves superior results across different model sizes, maximum lengths, and tasks. Our code will be made public at https://github.com/zerolllin/Delta-L-Normalization.

서로 다른 응답 길이에 대응하기 위한 보다 나은 Loss Normalization.

Better loss normalization for dealing with variable response lengths.

#rl #reasoning 