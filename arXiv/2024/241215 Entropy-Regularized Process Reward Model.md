https://arxiv.org/abs/2412.11006

*Entropy-Regularized Process Reward Model* (Hanning Zhang, Pengcheng Wang, Shizhe Diao, Yong Lin, Rui Pan, Hanze Dong, Dylan Zhang, Pavlo Molchanov, Tong Zhang)

> Large language models (LLMs) have shown promise in performing complex multi-step reasoning, yet they continue to struggle with mathematical reasoning, often making systematic errors. A promising solution is reinforcement learning (RL) guided by reward models, particularly those focusing on process rewards, which score each intermediate step rather than solely evaluating the final outcome. This approach is more effective at guiding policy models towards correct reasoning trajectories. In this work, we propose an entropy-regularized process reward model (ER-PRM) that integrates KL-regularized Markov Decision Processes (MDP) to balance policy optimization with the need to prevent the policy from shifting too far from its initial distribution. We derive a novel reward construction method based on the theoretical results. Our theoretical analysis shows that we could derive the optimal reward model from the initial policy sampling. Our empirical experiments on the MATH and GSM8K benchmarks demonstrate that ER-PRM consistently outperforms existing process reward models, achieving 1% improvement on GSM8K and 2-3% improvement on MATH under best-of-N evaluation, and more than 1% improvement under RLHF. These results highlight the efficacy of entropy-regularization in enhancing LLMs' reasoning capabilities.

정답을 사용한 PRM 학습에서 KL Penalty를 사용하기 위한 방법. 얼마 전 연구와 비슷한데 (https://arxiv.org/abs/2412.01981) Parameterization에서 차이가 있군요.

<english>
The method for using KL penalty in PRM training that uses outcome correctness. It is similar to recent research (https://arxiv.org/abs/2412.01981) but it is different in parameterization.
</english>

#reward-model

# Links

[[241202 Free Process Rewards without Process Labels.md]]