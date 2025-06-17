https://arxiv.org/abs/2408.03865

*PackMamba: Efficient Processing of Variable-Length Sequences in Mamba training* (Haoran Xu, Ziqian Liu, Rong Fu, Zhongling Su, Zerui Wang, Zheng Cai, Zhilin Pei, Xingcheng Zhang)

> With the evolution of large language models, traditional Transformer models become computationally demanding for lengthy sequences due to the quadratic growth in computation with respect to the sequence length. Mamba, emerging as a groundbreaking architecture in the field of generative AI, demonstrates remarkable proficiency in handling elongated sequences with reduced computational and memory complexity. Nevertheless, the existing training framework of Mamba presents inefficiency with variable-length sequence inputs. Either single-sequence training results in low GPU utilization, or batched processing of variable-length sequences to a maximum length incurs considerable memory and computational overhead. To address this problem, we analyze the performance of bottleneck operators in Mamba under diverse tensor shapes and proposed PackMamba, a high-throughput Mamba that efficiently handles variable-length sequences. Diving deep into state-space models (SSMs), we modify the parallel operators to avoid passing information between individual sequences while maintaining high performance. Experimental results on an NVIDIA A100 GPU demonstrate throughput exceeding the baseline single-sequence processing scheme: 3.06x speedup on the 1.4B model and 2.62x on the 2.8B model.

Mamba를 Packing된 시퀀스에 대해 학습하면서 이전 시퀀스의 상태로 이후 시퀀스가 영향을 받는 것을 막으려는 방법. Mamba 같은 경우 Packing에서 이전 시퀀스의 영향을 막는 것이 트랜스포머 보다 더 중요할 수 있다는 결과가 있었죠. (https://arxiv.org/abs/2406.07887)

State Space Model를 사용해야 하는가라는 문제 자체에 대해서는 최근 트랜스포머에서 Attention 캐시를 줄일 수 있는 방법들이 많이 등장하면서 이런 캐시 효율성 차원에서의 State Space Model의 장점은 바랬다는 느낌이 있습니다. 이전에도 그랬지만 State Space Model이 가지는 트랜스포머와는 다른 Inductive Bias의 측면이 더 흥미로울 것일 듯 합니다.

#efficient-training #state-space-model

# Links

[[240612 An Empirical Study of Mamba-based Language Models.md]]