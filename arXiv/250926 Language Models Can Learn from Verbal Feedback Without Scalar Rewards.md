https://arxiv.org/abs/2509.22638

*Language Models Can Learn from Verbal Feedback Without Scalar Rewards* (Renjie Luo, Zichen Liu, Xiangyan Liu, Chao Du, Min Lin, Wenhu Chen, Wei Lu, Tianyu Pang)

> LLMs are often trained with RL from human or AI feedback, yet such methods typically compress nuanced feedback into scalar rewards, discarding much of their richness and inducing scale imbalance. We propose treating verbal feedback as a conditioning signal. Inspired by language priors in text-to-image generation, which enable novel outputs from unseen prompts, we introduce the feedback-conditional policy (FCP). FCP learns directly from response-feedback pairs, approximating the feedback-conditional posterior through maximum likelihood training on offline data. We further develop an online bootstrapping stage where the policy generates under positive conditions and receives fresh feedback to refine itself. This reframes feedback-driven learning as conditional generation rather than reward optimization, offering a more expressive way for LLMs to directly learn from verbal feedback. Our code is available at https://github.com/sail-sg/feedback-conditional-policy.

스칼라 보상 대신 자연어 피드백을 사용해 LM을 튜닝. 피드백을 어디선가 가져올 필요가 있음. Principle 기반 Reward Model처럼 프롬프트에 대해 피드백을 생성하도록 학습하는 것이 가능할지?

Using natural language feedback to tune the language model instead of scalar rewards. Feedback needs to be obtained from somewhere. But would it be possible to learn to generate feedback conditioned on prompts, as in principle-based reward models?

#rl #reward-model 