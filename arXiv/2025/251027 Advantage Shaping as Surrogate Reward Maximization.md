https://arxiv.org/abs/2510.23049

*Advantage Shaping as Surrogate Reward Maximization: Unifying Pass@K Policy Gradients* (Christos Thrampoulidis, Sadegh Mahdavi, Wenlong Deng)

> This note reconciles two seemingly distinct approaches to policy gradient optimization for the Pass@K objective in reinforcement learning with verifiable rewards: (1) direct REINFORCE-style methods, and (2) advantage-shaping techniques that directly modify GRPO. We show that these are two sides of the same coin. By reverse-engineering existing advantage-shaping algorithms, we reveal that they implicitly optimize surrogate rewards. We specifically interpret practical ``hard-example up-weighting'' modifications to GRPO as reward-level regularization. Conversely, starting from surrogate reward objectives, we provide a simple recipe for deriving both existing and new advantage-shaping methods. This perspective provides a lens for RLVR policy gradient optimization beyond our original motivation of Pass@K.

Pass@K 학습에 대한 분석. Pass@K 학습을 위한 Advantage Shaping이 Pass@K의 Surrogate Reward의 최대화와 어떻게 관련되는지, 그리고 어려운 샘플을 업샘플링 하는 것과 어떻게 관련되는지를 드러냄.

Analysis on pass@k training. This shows how advantage shaping for pass@k training relates to maximizing surrogate reward of pass@k, and how it relates to upsampling of harder samples.

#rl 