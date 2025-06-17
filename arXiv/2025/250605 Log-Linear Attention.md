https://arxiv.org/abs/2506.04761

*Log-Linear Attention* (Han Guo, Songlin Yang, Tarushii Goel, Eric P. Xing, Tri Dao, Yoon Kim)

> The attention mechanism in Transformers is an important primitive for accurate and scalable sequence modeling. Its quadratic-compute and linear-memory complexity however remain significant bottlenecks. Linear attention and state-space models enable linear-time, constant-memory sequence modeling and can moreover be trained efficiently through matmul-rich parallelization across sequence length. However, at their core these models are still RNNs, and thus their use of a fixed-size hidden state to model the context is a fundamental limitation. This paper develops log-linear attention, an attention mechanism that balances linear attention's efficiency and the expressiveness of softmax attention. Log-linear attention replaces the fixed-size hidden state with a logarithmically growing set of hidden states. We show that with a particular growth function, log-linear attention admits a similarly matmul-rich parallel form whose compute cost is log-linear in sequence length. Log-linear attention is a general framework and can be applied on top of existing linear attention variants. As case studies, we instantiate log-linear variants of two recent architectures -- Mamba-2 and Gated DeltaNet -- and find they perform well compared to their linear-time variants.

길이에 따라 메모리가 고정되거나 혹은 선형 증가하는 것이 아니라 로그 증가하게 만든 절충이군요. 다만 여전히 Linear Attention 계통의 방법은 하이브리드로 사용되었을 때의 성능이 중요하겠죠.

<english>
Instead of fixed or linearly increasing memory along length, middle point with logarithmically increasing memory. But still for linear attention methods performance when used in the hybrid models would be more important.
</english>

#state-space-model 