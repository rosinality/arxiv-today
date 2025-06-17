https://arxiv.org/abs/2405.18719

*Contextual Position Encoding: Learning to Count What's Important* (Olga Golovneva, Tianlu Wang, Jason Weston, Sainbayar Sukhbaatar)

> The attention mechanism is a critical component of Large Language Models (LLMs) that allows tokens in a sequence to interact with each other, but is order-invariant. Incorporating position encoding (PE) makes it possible to address by position, such as attending to the i-th token. However, current PE methods use token counts to derive position, and thus cannot generalize to higher levels of abstraction, such as attending to the i-th sentence. In this paper, we propose a new position encoding method, Contextual Position Encoding (CoPE), that allows positions to be conditioned on context by incrementing position only on certain tokens determined by the model. This allows more general position addressing such as attending to the $i$-th particular word, noun, or sentence. We show that CoPE can solve the selective copy, counting and Flip-Flop tasks where popular position embeddings fail, and improves perplexity on language modeling and coding tasks.

QK 행렬에 Sigmoid를 적용한 다음 Cumulative Sum을 해서 Attention bias로 적용하는 형태의 Positional Encoding. QK 행렬을 사용해 Positional Encoding으로 사용하는 것은 얼마 전 나온 CAPE (https://arxiv.org/abs/2405.14722) 와도 유사하네요.

트랜스포머의 많은 문제가 Positional Encoding에서 기인하죠. (https://arxiv.org/abs/2405.17399) 다만 대안적 Positional Encoding이 문제에 특화되어 있거나 효율적으로 계산하기 어렵다는 것이 문제이긴 하네요.

#positional-encoding

# Links

[[240523 CAPE.md]]