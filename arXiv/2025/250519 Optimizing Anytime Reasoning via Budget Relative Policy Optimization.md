https://arxiv.org/abs/2505.13438

*Optimizing Anytime Reasoning via Budget Relative Policy Optimization* (Penghui Qi, Zichen Liu, Tianyu Pang, Chao Du, Wee Sun Lee, Min Lin)

> Scaling test-time compute is crucial for enhancing the reasoning capabilities of large language models (LLMs). Existing approaches typically employ reinforcement learning (RL) to maximize a verifiable reward obtained at the end of reasoning traces. However, such methods optimize only the final performance under a large and fixed token budget, which hinders efficiency in both training and deployment. In this work, we present a novel framework, AnytimeReasoner, to optimize anytime reasoning performance, which aims to improve token efficiency and the flexibility of reasoning under varying token budget constraints. To achieve this, we truncate the complete thinking process to fit within sampled token budgets from a prior distribution, compelling the model to summarize the optimal answer for each truncated thinking for verification. This introduces verifiable dense rewards into the reasoning process, facilitating more effective credit assignment in RL optimization. We then optimize the thinking and summary policies in a decoupled manner to maximize the cumulative reward. Additionally, we introduce a novel variance reduction technique, Budget Relative Policy Optimization (BRPO), to enhance the robustness and efficiency of the learning process when reinforcing the thinking policy. Empirical results in mathematical reasoning tasks demonstrate that our method consistently outperforms GRPO across all thinking budgets under various prior distributions, enhancing both training and token efficiency.

추론의 길이를 효율화하기 위한 연구가 정말 많이 나오고 있고 앞으로도 많이 나올 것 같네요. (https://arxiv.org/abs/2505.11827, https://arxiv.org/abs/2505.13417, https://arxiv.org/abs/2505.13379, https://arxiv.org/abs/2505.13326, https://arxiv.org/abs/2505.12284)

이전 연구와 비슷하게 추론과 결론의 예산을 분리하고 (https://arxiv.org/abs/2505.05315) 각 추론의 길이에 따라 보상을 부여해서 Dense Reward를 제공하는 방법.

효율적인 추론에 대해서 생각해보게 되네요. 간명한 증명은 그렇지 않은 증명과는 접근 자체가 다른 경우가 많겠죠. 그런 요인은 어떻게 반영할 수 있을까요.

<english>
There a lot of studies on optimizing length of reasoning, and I expect more will come. (https://arxiv.org/abs/2505.11827, https://arxiv.org/abs/2505.13417, https://arxiv.org/abs/2505.13379, https://arxiv.org/abs/2505.13326, https://arxiv.org/abs/2505.12284)

Similar to previous research this method separates budget for reasoning and summary (https://arxiv.org/abs/2505.05315), and assign dense reward by set rewards for each reasoning lengths.

It makes me to think about efficient reasoning. Concise proof tend to have vastly different approach than proof that are not. How can we reflect these factors?
</english>

#reasoning #rl 
