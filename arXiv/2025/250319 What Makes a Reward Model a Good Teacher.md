https://arxiv.org/abs/2503.15477

*What Makes a Reward Model a Good Teacher? An Optimization Perspective* (Noam Razin, Zixuan Wang, Hubert Strauss, Stanley Wei, Jason D. Lee, Sanjeev Arora)

> The success of Reinforcement Learning from Human Feedback (RLHF) critically depends on the quality of the reward model. While this quality is primarily evaluated through accuracy, it remains unclear whether accuracy fully captures what makes a reward model an effective teacher. We address this question from an optimization perspective. First, we prove that regardless of how accurate a reward model is, if it induces low reward variance, then the RLHF objective suffers from a flat landscape. Consequently, even a perfectly accurate reward model can lead to extremely slow optimization, underperforming less accurate models that induce higher reward variance. We additionally show that a reward model that works well for one language model can induce low reward variance, and thus a flat objective landscape, for another. These results establish a fundamental limitation of evaluating reward models solely based on accuracy or independently of the language model they guide. Experiments using models of up to 8B parameters corroborate our theory, demonstrating the interplay between reward variance, accuracy, and reward maximization rate. Overall, our findings highlight that beyond accuracy, a reward model needs to induce sufficient variance for efficient optimization.

Reward Model은 정확도 뿐만 아니라 Policy가 생성한 샘플에 대한 Reward Score의 분산도 중요하다는 연구. 분산은 Policy도 영향을 미치기에 Policy와 Reward Model 모두의 특성이 중요해지죠.

<english>
The research insist not only accurate, but variance of reward scores for generated samples from policy is import for reward model. As policy affects variance, characteristics of policy and reward model are both become important.
</english>

#reward-model #rlhf 