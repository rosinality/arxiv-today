https://arxiv.org/abs/2412.01505

*Scaling Law for Language Models Training Considering Batch Size* (Xian Shuai, Yiding Wang, Yimeng Wu, Xin Jiang, Xiaozhe Ren)

> Large language models (LLMs) have made remarkable advances in recent years, with scaling laws playing a critical role in this rapid progress. In this paper, we empirically investigate how a critical hyper-parameter, i.e., the global batch size, influences the LLM training prdocess. We begin by training language models ranging from 125 million to 2.6 billion parameters, using up to 300 billion high-quality tokens. Through these experiments, we establish a basic scaling law on model size and training data amount. We then examine how varying batch sizes and learning rates affect the convergence and generalization of these models. Our analysis yields batch size scaling laws under two different cases: with a fixed compute budget, and with a fixed amount of training data. Extrapolation experiments on models of increasing sizes validate our predicted laws, which provides guidance for optimizing LLM training strategies under specific resource constraints.

연산량과 데이터의 증가에 따른 최적 배치 크기의 Scaling Law. 학습 규모 증가에 따라 수많은 노브들을 어떻게 조절해야 할 것인지는 정말 성가신 문제죠. (https://arxiv.org/abs/2409.15156)

<english>
Scaling law on optimal batch sizes along with increase of computation and data. It is very cumbersome problem to adjust various knobs with increasing training scales. (https://arxiv.org/abs/2409.15156)
</english>

#scaling-law #hyperparameter

# Links

[[240923 Rethinking Conventional Wisdom in Machine Learning.md]]