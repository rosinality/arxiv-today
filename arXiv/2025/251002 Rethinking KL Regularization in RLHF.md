https://arxiv.org/abs/2510.01555

*Rethinking KL Regularization in RLHF: From Value Estimation to Gradient Optimization* (Kezhao Liu, Jason Klein Liu, Mingtao Chen, Yiming Liu)

> Reinforcement Learning from Human Feedback (RLHF) leverages a Kullback-Leibler (KL) divergence loss to stabilize training and prevent overfitting. However, in methods such as GRPO, its implementation may be guided by principles from numerical value estimation-a practice that overlooks the term's functional role as an optimization loss. To analyze this issue, we establish a unified framework that connects two seemingly distinct implementation styles: using the mathematical term $k_n$ as a detached coefficient for the policy's score function ('$k_n$ in reward') or as a direct loss function through which gradients are propagated ('$k_n$ as loss'). We show that the latter can always be analyzed via an equivalent gradient coefficient in the former, unifying the two perspectives. Through this framework, we prove that the conventional '$k_1$ in reward' (like in PPO) is the principled loss for Reverse KL (RKL) regularization. We further establish a key finding: under on-policy conditions, the '$k_2$ as loss' formulation is, in fact, gradient-equivalent to '$k_1$ in reward'. This equivalence, first proven in our work, identifies both as the theoretically sound implementations of the RKL objective. In contrast, we show that the recently adopted '$k_3$ as loss' (like in GRPO) is merely a first-order, biased approximation of the principled loss. Furthermore, we argue that common off-policy implementations of '$k_n$ as loss' methods are biased due to neglected importance sampling, and we propose a principled correction. Our findings provide a comprehensive, gradient-based rationale for choosing and correctly implementing KL regularization, paving the way for more robust and effective RLHF systems.

KL Estimator k1, k2, k3와 이를 Reward 혹은 Loss로 사용하는 방법에 대한 분석. 부분적으로 이전에 있었던 논의의 연장 https://x.com/QuanquanGu/status/1972138059237150934.

RLHF라고 하고 있지만 실제로는 RLVR을 수행.

Analysis of KL estimator k1, k2, k3 and their use as a reward or as a loss. Partially this is a continuation of previous discussions on it https://x.com/QuanquanGu/status/1972138059237150934.

By the way RLHF is a bit misleading; they did RLVR.

#rl 