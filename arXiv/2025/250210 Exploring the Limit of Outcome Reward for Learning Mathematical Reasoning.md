https://arxiv.org/abs/2502.06781

*Exploring the Limit of Outcome Reward for Learning Mathematical Reasoning* (Chengqi Lyu, Songyang Gao, Yuzhe Gu, Wenwei Zhang, Jianfei Gao, Kuikun Liu, Ziyi Wang, Shuaibin Li, Qian Zhao, Haian Huang, Weihan Cao, Jiangning Liu, Hongwei Liu, Junnan Liu, Songyang Zhang, Dahua Lin, Kai Chen)

> Reasoning abilities, especially those for solving complex math problems, are crucial components of general intelligence. Recent advances by proprietary companies, such as o-series models of OpenAI, have made remarkable progress on reasoning tasks. However, the complete technical details remain unrevealed, and the techniques that are believed certainly to be adopted are only reinforcement learning (RL) and the long chain of thoughts. This paper proposes a new RL framework, termed OREAL, to pursue the performance limit that can be achieved through \textbf{O}utcome \textbf{RE}w\textbf{A}rd-based reinforcement \textbf{L}earning for mathematical reasoning tasks, where only binary outcome rewards are easily accessible. We theoretically prove that behavior cloning on positive trajectories from best-of-N (BoN) sampling is sufficient to learn the KL-regularized optimal policy in binary feedback environments. This formulation further implies that the rewards of negative samples should be reshaped to ensure the gradient consistency between positive and negative samples. To alleviate the long-existing difficulties brought by sparse rewards in RL, which are even exacerbated by the partial correctness of the long chain of thought for reasoning tasks, we further apply a token-level reward model to sample important tokens in reasoning trajectories for learning. With OREAL, for the first time, a 7B model can obtain 94.0 pass@1 accuracy on MATH-500 through RL, being on par with 32B models. OREAL-32B also surpasses previous 32B models trained by distillation with 95.0 pass@1 accuracy on MATH-500. Our investigation also indicates the importance of initial policy models and training queries for RL. Code, models, and data will be released to benefit future research\footnote{https://github.com/InternLM/OREAL}.

Binary Feedback 상황에서 BoN 샘플이 KL penalized Optimal Policy 학습에 충분하다는 것을 기반으로, Negative 샘플을 고려한 Reward shaping과 단순한 Token level reward model을 사용한 학습.

KL penalty를 사용한다고 생각하면 BoN과 연결하는 것은 자연스럽죠. 그런 의미에서 RL CoT 문제에 대해서 KL penalty의 효과를 이해하는 것이 중요하다고 생각합니다.

<english>
Based on the sufficiency of BoN sample to train KL-penalized optimal policy on binary feedbacks, trained a RL CoT model with reward shaping for negative samples and simple token level reward models.

It is natural to connect RL to BoN when KL penalty is applied. In that sense I think it is important to understand effect of KL penalty for RL CoT task.
</english>

#reasoning #rl 