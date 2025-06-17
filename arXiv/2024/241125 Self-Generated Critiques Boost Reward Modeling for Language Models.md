https://arxiv.org/abs/2411.16646

*Self-Generated Critiques Boost Reward Modeling for Language Models* (Yue Yu, Zhengxing Chen, Aston Zhang, Liang Tan, Chenguang Zhu, Richard Yuanzhe Pang, Yundi Qian, Xuewei Wang, Suchin Gururangan, Chao Zhang, Melanie Kambadur, Dhruv Mahajan, Rui Hou)

> Reward modeling is crucial for aligning large language models (LLMs) with human preferences, especially in reinforcement learning from human feedback (RLHF). However, current reward models mainly produce scalar scores and struggle to incorporate critiques in a natural language format. We hypothesize that predicting both critiques and the scalar reward would improve reward modeling ability. Motivated by this, we propose Critic-RM, a framework that improves reward models using self-generated critiques without extra supervision. Critic-RM employs a two-stage process: generating and filtering high-quality critiques, followed by joint fine-tuning on reward prediction and critique generation. Experiments across benchmarks show that Critic-RM improves reward modeling accuracy by 3.7%-7.3% compared to standard reward models and LLM judges, demonstrating strong performance and data efficiency. Additional studies further validate the effectiveness of generated critiques in rectifying flawed reasoning steps with 2.5%-3.2% gains in improving reasoning accuracy.

Critique을 생성하는 Reward Model. Reward Score 예측 + Critique을 생성한 다음 Preference Label을 사용한 필터링과 LLM을 사용한 개선 결과를 사용해 Critique 학습.

<english>
Reward model that generates critique. Training model to generate a critique by predicting reward scores and training on critiques synthesized by applying filtering and refinement using LLMs to sampled critiques from the model.
</english>

#reward-model 