https://arxiv.org/abs/2402.00856

*Towards Efficient and Exact Optimization of Language Model Alignment* (Haozhe Ji, Cheng Lu, Yilin Niu, Pei Ke, Hongning Wang, Jun Zhu, Jie Tang, Minlie Huang)

> The alignment of language models with human preferences is vital for their application in real-world tasks. The problem is formulated as optimizing the model's policy to maximize the expected reward that reflects human preferences with minimal deviation from the initial policy. While considered as a straightforward solution, reinforcement learning (RL) suffers from high variance in policy updates, which impedes efficient policy improvement. Recently, direct preference optimization (DPO) was proposed to directly optimize the policy from preference data. Though simple to implement, DPO is derived based on the optimal policy that is not assured to be achieved in practice, which undermines its convergence to the intended solution. In this paper, we propose efficient exact optimization (EXO) of the alignment objective. We prove that EXO is guaranteed to optimize in the same direction as the RL algorithms asymptotically for arbitary parametrization of the policy, while enables efficient optimization by circumventing the complexities associated with RL algorithms. We compare our method to DPO with both theoretical and empirical analyses, and further demonstrate the advantages of our method over existing approaches on realistic human preference data.

DPO + Reverse KL + Reward Model을 통해 K개 샘플을 사용이라는 느낌이군요.

#rlhf 

It seems like DPO + Reverse KL + Using K sample by utilizing Reward Model.