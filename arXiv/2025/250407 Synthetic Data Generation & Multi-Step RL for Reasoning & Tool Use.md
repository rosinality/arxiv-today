https://arxiv.org/abs/2504.04736

*Synthetic Data Generation & Multi-Step RL for Reasoning & Tool Use* (Anna Goldie, Azalia Mirhoseini, Hao Zhou, Irene Cai, Christopher D. Manning)

> Reinforcement learning has been shown to improve the performance of large language models. However, traditional approaches like RLHF or RLAIF treat the problem as single-step. As focus shifts toward more complex reasoning and agentic tasks, language models must take multiple steps of text generation, reasoning and environment interaction before generating a solution. We propose a synthetic data generation and RL methodology targeting multi-step optimization scenarios. This approach, called Step-Wise Reinforcement Learning (SWiRL), iteratively generates multi-step reasoning and tool use data, and then learns from that data. It employs a simple step-wise decomposition that breaks each multi-step trajectory into multiple sub-trajectories corresponding to each action by the original model. It then applies synthetic data filtering and RL optimization on these sub-trajectories. We evaluated SWiRL on a number of multi-step tool use, question answering, and mathematical reasoning tasks. Our experiments show that SWiRL outperforms baseline approaches by 21.5%, 12.3%, 14.8%, 11.1%, and 15.3% in relative accuracy on GSM8K, HotPotQA, CofCA, MuSiQue, and BeerQA, respectively. Excitingly, the approach exhibits generalization across tasks: for example, training only on HotPotQA (text question-answering) improves zero-shot performance on GSM8K (a math dataset) by a relative 16.9%.

Multi Step 도구 사용과 추론을 위한 데이터 생성과 RL 방법. 그런데 Ground Truth 사용 없이 Reward Model만으로 액션만을 평가하는 형태군요.

<english>
The method for synthesizing data and RL for multi step tool use and reasoning. But they did not use ground truth and only evaluates action with reward models.
</english>

#rl #reasoning #tool #synthetic-data 