https://arxiv.org/abs/2505.16381

*PaTH Attention: Position Encoding via Accumulating Householder Transformations* (Songlin Yang, Yikang Shen, Kaiyue Wen, Shawn Tan, Mayank Mishra, Liliang Ren, Rameswar Panda, Yoon Kim)

> The attention mechanism is a core primitive in modern large language models (LLMs) and AI more broadly. Since attention by itself is permutation-invariant, position encoding is essential for modeling structured domains such as language. Rotary position encoding (RoPE) has emerged as the de facto standard approach for position encoding and is part of many modern LLMs. However, in RoPE the key/query transformation between two elements in a sequence is only a function of their relative position and otherwise independent of the actual input. This limits the expressivity of RoPE-based transformers. This paper describes PaTH, a flexible data-dependent position encoding scheme based on accumulated products of Householder(like) transformations, where each transformation is data-dependent, i.e., a function of the input. We derive an efficient parallel algorithm for training through exploiting a compact representation of products of Householder matrices, and implement a FlashAttention-style blockwise algorithm that minimizes I/O cost. Across both targeted synthetic benchmarks and moderate-scale real-world language modeling experiments, we find that PaTH demonstrates superior performance compared to RoPE and other recent baselines.

두 토큰 사이의 토큰들에서 계산한 게이트 값의 곱으로 Position Encoding을 계산. Stick-Breaking Attention 생각이 나는군요 (https://arxiv.org/abs/2410.17980).

<english>
Calculating position encoding by multiplying gate values from the tokens between two tokens. It reminds me stick-breaking attention (https://arxiv.org/abs/2410.17980).
</english>

#attention #transformer 