https://arxiv.org/abs/2412.17747

*Deliberation in Latent Space via Differentiable Cache Augmentation* (Luyang Liu, Jonas Pfeiffer, Jiaxing Wu, Jun Xie, Arthur Szlam)

> Techniques enabling large language models (LLMs) to "think more" by generating and attending to intermediate reasoning steps have shown promise in solving complex problems. However, the standard approaches generate sequences of discrete tokens immediately before responding, and so they can incur significant latency costs and be challenging to optimize. In this work, we demonstrate that a frozen LLM can be augmented with an offline coprocessor that operates on the model's key-value (kv) cache. This coprocessor augments the cache with a set of latent embeddings designed to improve the fidelity of subsequent decoding. We train this coprocessor using the language modeling loss from the decoder on standard pretraining data, while keeping the decoder itself frozen. This approach enables the model to learn, in an end-to-end differentiable fashion, how to distill additional computation into its kv-cache. Because the decoder remains unchanged, the coprocessor can operate offline and asynchronously, and the language model can function normally if the coprocessor is unavailable or if a given cache is deemed not to require extra computation. We show experimentally that when a cache is augmented, the decoder achieves lower perplexity on numerous subsequent tokens. Furthermore, even without any task-specific training, our experiments demonstrate that cache augmentation consistently reduces perplexity and improves performance across a range of reasoning-intensive tasks.

Continuous 토큰을 추론 토큰으로 사용할 수 있게 하는 아키텍처. KV 캐시를 Coprocessor 모델에 넘기고 소프트 토큰을 입력으로 해서 추가 KV 캐시 임베딩을 만들어서 다음 토큰 예측에 활용하는 형태입니다. Pause 토큰과 (https://arxiv.org/abs/2310.02226) 비슷한데 여기서는 Coprocessor 모델을 추가로 통과한다는 차이가 있겠네요.

Discrete 토큰보다 Continuous 토큰이 더 많은 표현력을 갖겠지만 그걸 어떻게 학습시킬 수 있는가가 문제가 되겠죠. (https://arxiv.org/abs/2412.06769) 여기서도 Teacher Forcing을 사용할 수는 없었죠.

<english>
Architecture that allows continuous token as reasoning tokens. Overall method is first generate additional KV cache embeddings by using coprocessor model with KV cache and soft token as an input, and utilizing it for next token prediction. It is similar to pause tokens (https://arxiv.org/abs/2310.02226) but this model uses additional coprocessor model to embed pause tokens.

Continuous token would have better representational capacity than discrete tokens but how can we train it would be the problem (https://arxiv.org/abs/2412.06769). This work was also not able to use teacher forcing to train the continuous tokens.
</english>

#reasoning #transformer

# Links

[[241209 Training Large Language Models to Reason in a Continuous Latent Space.md]]
[[231003 Think before you speak.md]]