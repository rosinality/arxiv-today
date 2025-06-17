https://arxiv.org/abs/2410.01679

*VinePPO: Unlocking RL Potential For LLM Reasoning Through Refined Credit Assignment* (Amirhossein Kazemnejad, Milad Aghajohari, Eva Portelance, Alessandro Sordoni, Siva Reddy, Aaron Courville, Nicolas Le Roux)

> Large language models (LLMs) are increasingly applied to complex reasoning tasks that require executing several complex steps before receiving any reward. Properly assigning credit to these steps is essential for enhancing model performance. Proximal Policy Optimization (PPO), a state-of-the-art reinforcement learning (RL) algorithm used for LLM finetuning, employs value networks to tackle credit assignment. However, value networks face challenges in predicting the expected cumulative rewards accurately in complex reasoning tasks, often leading to high-variance updates and suboptimal performance. In this work, we systematically evaluate the efficacy of value networks and reveal their significant shortcomings in reasoning-heavy LLM tasks, showing that they barely outperform a random baseline when comparing alternative steps. To address this, we propose VinePPO, a straightforward approach that leverages the flexibility of language environments to compute unbiased Monte Carlo-based estimates, bypassing the need for large value networks. Our method consistently outperforms PPO and other RL-free baselines across MATH and GSM8K datasets with fewer gradient updates (up to 9x), less wall-clock time (up to 3.0x). These results emphasize the importance of accurate credit assignment in RL finetuning of LLM and demonstrate VinePPO's potential as a superior alternative.

추론 과제에 대해 RL을 진행할 때 추론 과정에서 중요한 지점을 Value Function이 찾아내야 하는데 보통 그러지 못한다는 지적. 이를 샘플링을 통한 Monte Carlo 추정으로 대체한다는 아이디어입니다. Value Function을 샘플링으로 대체하는 것은 GRPO와도 비슷하네요. (https://arxiv.org/abs/2402.03300)

<english>
During RL for reasoning tasks it is crucial to value function to find important reasoning steps, but it is commonly fail to do so. So this work tries to replate it with monte carlo estimate by sampling. The idea that replaces value function with sampling is similar to GRPO. (https://arxiv.org/abs/2402.03300)
</english>

#reasoning #rl

# Links

[[240205 DeepSeekMath.md]]