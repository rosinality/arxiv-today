https://arxiv.org/abs/2404.14367

*Preference Fine-Tuning of LLMs Should Leverage Suboptimal, On-Policy Data* (Fahim Tajwar, Anikait Singh, Archit Sharma, Rafael Rafailov, Jeff Schneider, Tengyang Xie, Stefano Ermon, Chelsea Finn, Aviral Kumar)

> Learning from preference labels plays a crucial role in fine-tuning large language models. There are several distinct approaches for preference fine-tuning, including supervised learning, on-policy reinforcement learning (RL), and contrastive learning. Different methods come with different implementation tradeoffs and performance differences, and existing empirical findings present different conclusions, for instance, some results show that online RL is quite important to attain good fine-tuning results, while others find (offline) contrastive or even purely supervised methods sufficient. This raises a natural question: what kind of approaches are important for fine-tuning with preference data and why? In this paper, we answer this question by performing a rigorous analysis of a number of fine-tuning techniques on didactic and full-scale LLM problems. Our main finding is that, in general, approaches that use on-policy sampling or attempt to push down the likelihood on certain responses (i.e., employ a "negative gradient") outperform offline and maximum likelihood objectives. We conceptualize our insights and unify methods that use on-policy sampling or negative gradient under a notion of mode-seeking objectives for categorical distributions. Mode-seeking objectives are able to alter probability mass on specific bins of a categorical distribution at a fast rate compared to maximum likelihood, allowing them to relocate masses across bins more effectively. Our analysis prescribes actionable insights for preference fine-tuning of LLMs and informs how data should be collected for maximal improvement.

RLHF 방법들의 논쟁점들, On Policy vs Off Policy, Negative Gradient (Likelihood)를 사용할 것인가의 문제에 대한 종합적인 분석이군요. On Policy와 Negative Gradient를 사용하는 쪽이 효과적이라는 결론입니다.

On Policy, Negative Gradient가 레퍼런스 분포에 비해 Reward의 피크 분포가 멀리 떨어져 있을 때 효과적인데 이는 이 두 방법이 Reverse KL Objective이고 따라서 Mode Seeking이기 때문입니다. 반대로 그렇지 않은 방법은 Mode Covering을 하게 되죠.

PPO를 진행할 때 Diversity가 감소하는 특성 등을 고려하면 자연스러운 흐름이긴 합니다.

#rlhf 