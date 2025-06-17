https://arxiv.org/abs/2505.10425

*Learning to Think: Information-Theoretic Reinforcement Fine-Tuning for LLMs* (Jingyao Wang, Wenwen Qiang, Zeen Song, Changwen Zheng, Hui Xiong)

> Large language models (LLMs) excel at complex tasks thanks to advances in reasoning abilities. However, existing methods overlook the trade-off between reasoning effectiveness and computational efficiency, often encouraging unnecessarily long reasoning chains and wasting tokens. To address this, we propose Learning to Think (L2T), an information-theoretic reinforcement fine-tuning framework for LLMs to make the models achieve optimal reasoning with fewer tokens. Specifically, L2T treats each query-response interaction as a hierarchical session of multiple episodes and proposes a universal dense process reward, i.e., quantifies the episode-wise information gain in parameters, requiring no extra annotations or task-specific evaluators. We propose a method to quickly estimate this reward based on PAC-Bayes bounds and the Fisher information matrix. Theoretical analyses show that it significantly reduces computational complexity with high estimation accuracy. By immediately rewarding each episode's contribution and penalizing excessive updates, L2T optimizes the model via reinforcement learning to maximize the use of each episode and achieve effective updates. Empirical results on various reasoning benchmarks and base models demonstrate the advantage of L2T across different tasks, boosting both reasoning effectiveness and efficiency.

추론 과정을 에피소드들로 나누고 각 에피소드들이 정답률 향상에 얼마나 기여하는지를 통해 추론 효율성을 향상. 이전 연구와 비슷한데 (https://arxiv.org/abs/2503.07572) 파라미터에 대한 페널티를 추가로 사용하는군요.

<english>
Improve reasoning efficiency by splitting reasoning processes into episodes and estimate how each episodes contributed to improvement of accuracy. It is similar to previous research (https://arxiv.org/abs/2503.07572) and this study uses additional penalty on parameters.
</english>

#rl #reasoning #reward 