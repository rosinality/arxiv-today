https://arxiv.org/abs/2504.18458

*Fast-Slow Thinking for Large Vision-Language Model Reasoning* (Wenyi Xiao, Leilei Gan, Weilong Dai, Wanggui He, Ziwei Huang, Haoyuan Li, Fangxun Shu, Zhelun Yu, Peng Zhang, Hao Jiang, Fei Wu)

> Recent advances in large vision-language models (LVLMs) have revealed an \textit{overthinking} phenomenon, where models generate verbose reasoning across all tasks regardless of questions. To address this issue, we present \textbf{FAST}, a novel \textbf{Fa}st-\textbf{S}low \textbf{T}hinking framework that dynamically adapts reasoning depth based on question characteristics. Through empirical analysis, we establish the feasibility of fast-slow thinking in LVLMs by investigating how response length and data distribution affect performance. We develop FAST-GRPO with three components: model-based metrics for question characterization, an adaptive thinking reward mechanism, and difficulty-aware KL regularization. Experiments across seven reasoning benchmarks demonstrate that FAST achieves state-of-the-art accuracy with over 10\% relative improvement compared to the base model, while reducing token usage by 32.7-67.3\% compared to previous slow-thinking approaches, effectively balancing reasoning length and accuracy.

GRPO에서 샘플의 길이 증가와 문제의 난이도를 연결한 연구가 나왔군요. (https://arxiv.org/abs/2504.05185) 이쪽도 비슷하게 어려운 난이도로 시작해서 쉬운 난이도로 마무리하는 방식이네요.

<english>
The study of connecting increasement of length of samples and difficulty of the problem in GRPO (https://arxiv.org/abs/2504.05185). Similar to previous tudy, this study also suggest to start the train from hard problems and ends with easier problems.
</english>

#rl #reasoning 