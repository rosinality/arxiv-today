https://arxiv.org/abs/2504.04950

*A Unified Pairwise Framework for RLHF: Bridging Generative Reward Modeling and Policy Optimization* (Wenyuan Xu, Xiaochen Zuo, Chao Xin, Yu Yue, Lin Yan, Yonghui Wu)

> Reinforcement Learning from Human Feedback (RLHF) has emerged as a important paradigm for aligning large language models (LLMs) with human preferences during post-training. This framework typically involves two stages: first, training a reward model on human preference data, followed by optimizing the language model using reinforcement learning algorithms. However, current RLHF approaches may constrained by two limitations. First, existing RLHF frameworks often rely on Bradley-Terry models to assign scalar rewards based on pairwise comparisons of individual responses. However, this approach imposes significant challenges on reward model (RM), as the inherent variability in prompt-response pairs across different contexts demands robust calibration capabilities from the RM. Second, reward models are typically initialized from generative foundation models, such as pre-trained or supervised fine-tuned models, despite the fact that reward models perform discriminative tasks, creating a mismatch. This paper introduces Pairwise-RL, a RLHF framework that addresses these challenges through a combination of generative reward modeling and a pairwise proximal policy optimization (PPO) algorithm. Pairwise-RL unifies reward model training and its application during reinforcement learning within a consistent pairwise paradigm, leveraging generative modeling techniques to enhance reward model performance and score calibration. Experimental evaluations demonstrate that Pairwise-RL outperforms traditional RLHF frameworks across both internal evaluation datasets and standard public benchmarks, underscoring its effectiveness in improving alignment and model behavior.

Principle과 응답 페어를 입력으로 사용하는 Generative Reward Model과 Pairwise PPO의 결합. RLHF 쪽은 비슷한 방향으로 흘러가고 있네요.

<english>
Combination of generative reward model that uses principle and response pairs, and pairwise PPO. RLHF are progressing in similar directions.
</english>

#rlhf #reward-model 