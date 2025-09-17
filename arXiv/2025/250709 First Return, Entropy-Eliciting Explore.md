https://arxiv.org/abs/2507.07017

*First Return, Entropy-Eliciting Explore* (Tianyu Zheng, Tianshun Xing, Qingshui Gu, Taoran Liang, Xingwei Qu, Xin Zhou, Yizhi Li, Zhoufutu Wen, Chenghua Lin, Wenhao Huang, Qian Liu, Ge Zhang, Zejun Ma)

> Reinforcement Learning from Verifiable Rewards (RLVR) improves the reasoning abilities of Large Language Models (LLMs) but it struggles with unstable exploration. We propose FR3E (First Return, Entropy-Eliciting Explore), a structured exploration framework that identifies high-uncertainty decision points in reasoning trajectories and performs targeted rollouts to construct semantically grounded intermediate feedback. Our method provides targeted guidance without relying on dense supervision. Empirical results on mathematical reasoning benchmarks(AIME24) show that FR3E promotes more stable training, produces longer and more coherent responses, and increases the proportion of fully correct trajectories. These results highlight the framework's effectiveness in improving LLM reasoning through more robust and structured exploration.

엔트로피가 높은 토큰이 보통 분기점이므로 그 지점에서 추가적인 롤아웃을 생성해서 탐색을 촉진할 수 있다는 연구군요 (https://arxiv.org/abs/2506.01939).

<english>
A study for enhancing exploration by generating additional rollouts at the token with high entropy, because usually it is point of branches (https://arxiv.org/abs/2506.01939).
</english>

#rl #reasoning 