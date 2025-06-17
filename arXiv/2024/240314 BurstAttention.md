https://arxiv.org/abs/2403.09347

*BurstAttention: An Efficient Distributed Attention Framework for Extremely Long Sequences* (Sun Ao, Weilin Zhao, Xu Han, Cheng Yang, Zhiyuan Liu, Chuan Shi, Maosong Sun, Shengnan Wang, Teng Su)

> Effective attention modules have played a crucial role in the success of Transformer-based large language models (LLMs), but the quadratic time and memory complexities of these attention modules also pose a challenge when processing long sequences. One potential solution for the long sequence problem is to utilize distributed clusters to parallelize the computation of attention modules across multiple devices (e.g., GPUs). However, adopting a distributed approach inevitably introduces extra memory overheads to store local attention results and incurs additional communication costs to aggregate local results into global ones. In this paper, we propose a distributed attention framework named ``BurstAttention'' to optimize memory access and communication operations at both the global cluster and local device levels. In our experiments, we compare BurstAttention with other competitive distributed attention solutions for long sequence processing. The experimental results under different length settings demonstrate that BurstAttention offers significant advantages for processing long sequences compared with these competitive baselines, reducing 40% communication overheads and achieving 2 X speedup during training 32K sequence length on 8 X A100.

Distributed Attention에 대한 최적화. 사실 Ring Attention (https://arxiv.org/abs/2310.01889) 에서 Jax/Pallas로 작업한 Online Softmax 기반의 구현 방식과 비슷한 작업으로 보이네요.

#efficient-training

# Links

