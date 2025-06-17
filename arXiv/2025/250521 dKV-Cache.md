https://arxiv.org/abs/2505.15781

*dKV-Cache: The Cache for Diffusion Language Models* (Xinyin Ma, Runpeng Yu, Gongfan Fang, Xinchao Wang)

> Diffusion Language Models (DLMs) have been seen as a promising competitor for autoregressive language models. However, diffusion language models have long been constrained by slow inference. A core challenge is that their non-autoregressive architecture and bidirectional attention preclude the key-value cache that accelerates decoding. We address this bottleneck by proposing a KV-cache-like mechanism, delayed KV-Cache, for the denoising process of DLMs. Our approach is motivated by the observation that different tokens have distinct representation dynamics throughout the diffusion process. Accordingly, we propose a delayed and conditioned caching strategy for key and value states. We design two complementary variants to cache key and value step-by-step: (1) dKV-Cache-Decode, which provides almost lossless acceleration, and even improves performance on long sequences, suggesting that existing DLMs may under-utilise contextual information during inference. (2) dKV-Cache-Greedy, which has aggressive caching with reduced lifespan, achieving higher speed-ups with quadratic time complexity at the cost of some performance degradation. dKV-Cache, in final, achieves from 2-10x speedup in inference, largely narrowing the gap between ARs and DLMs. We evaluate our dKV-Cache on several benchmarks, delivering acceleration across general language understanding, mathematical, and code-generation benchmarks. Experiments demonstrate that cache can also be used in DLMs, even in a training-free manner from current DLMs.

Diffusion LM에 대해 KV 캐시가 가능한지를 시도했군요. 토큰을 예측한 다음에는 KV 임베딩이 크게 변화하지 않는다는 것을 활용했다고. Causal LM처럼 학습 방식 자체가 KV 캐시를 허용하는 방법이 가능할까요.

<english>
Attempt on feasibility of KV cache for diffusion LM. They utilized tendency of KV embedding does not change much after token is predicted. Would it possible to find out training objective itself allows KV cache, like causal LM?
</english>

#diffusion #lm #efficiency 