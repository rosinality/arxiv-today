https://arxiv.org/abs/2405.12981

*Reducing Transformer Key-Value Cache Size with Cross-Layer Attention* (William Brandon, Mayank Mishra, Aniruddha Nrusimha, Rameswar Panda, Jonathan Ragan Kelly)

> Key-value (KV) caching plays an essential role in accelerating decoding for transformer-based autoregressive large language models (LLMs). However, the amount of memory required to store the KV cache can become prohibitive at long sequence lengths and large batch sizes. Since the invention of the transformer, two of the most effective interventions discovered for reducing the size of the KV cache have been Multi-Query Attention (MQA) and its generalization, Grouped-Query Attention (GQA). MQA and GQA both modify the design of the attention block so that multiple query heads can share a single key/value head, reducing the number of distinct key/value heads by a large factor while only minimally degrading accuracy. In this paper, we show that it is possible to take Multi-Query Attention a step further by also sharing key and value heads between adjacent layers, yielding a new attention design we call Cross-Layer Attention (CLA). With CLA, we find that it is possible to reduce the size of the KV cache by another 2x while maintaining nearly the same accuracy as unmodified MQA. In experiments training 1B- and 3B-parameter models from scratch, we demonstrate that CLA provides a Pareto improvement over the memory/accuracy tradeoffs which are possible with traditional MQA, enabling inference with longer sequence lengths and larger batch sizes than would otherwise be possible

하나의 KV 캐시를 여러 레이어에서 공유해서 KV 캐시의 크기를 줄이는 방법. 얼마 전 Cross Attention을 사용해 인코더 임베딩처럼 사용한 방법과 비슷하네요. (https://arxiv.org/abs/2405.05254)

KV 캐시에 대한 압축 방법이 꽤 많이 등장하고 있고 DeepSeek V2의 MLA (https://arxiv.org/abs/2405.04434) 같은 경우 성능적으로도 흥미로운 가능성을 보여주고 있죠. 여담이지만 KV 캐시의 압축률이 높아질수록 State Space Model이 갖는 상태 크기에서의 이점이 압착되고 있긴 합니다.

#efficiency

# Links

[[240508 You Only Cache Once.md]]