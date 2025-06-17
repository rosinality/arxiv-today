https://arxiv.org/abs/2411.13476

*When Precision Meets Position: BFloat16 Breaks Down RoPE in Long-Context Training* (Haonan Wang, Qian Liu, Chao Du, Tongyao Zhu, Cunxiao Du, Kenji Kawaguchi, Tianyu Pang)

> Extending context window sizes allows large language models (LLMs) to process longer sequences and handle more complex tasks. Rotary Positional Embedding (RoPE) has become the de facto standard due to its relative positional encoding properties that benefit long-context training. However, we observe that using RoPE with BFloat16 format results in numerical issues, causing it to deviate from its intended relative positional encoding, especially in long-context scenarios. This issue arises from BFloat16's limited precision and accumulates as context length increases, with the first token contributing significantly to this problem. To address this, we develop AnchorAttention, a plug-and-play attention method that alleviates numerical issues caused by BFloat16, improves long-context capabilities, and speeds up training. AnchorAttention reduces unnecessary attention computations, maintains semantic coherence, and boosts computational efficiency by treating the first token as a shared anchor with a consistent position ID, making it visible to all documents within the training context. Experiments on three types of LLMs demonstrate that AnchorAttention significantly improves long-context performance and reduces training time by over 50\% compared to standard full attention mechanisms, while preserving the original LLM's capabilities on general tasks. Our code is available at https://github.com/haonan3/AnchorContext.

BFloat16 + RoPE에서 발생하는 문제. 분석이 좀 많습니다. Long Context 문제를 태클하다가 발견한 것이 아닌가 싶네요.

BFloat16으로 RoPE를 사용하면 RoPE의 Relative Positional Encoding으로서의 효과가 떨어진다는 것이 요점입니다. 즉 위치를 이동하면 Attention이 크게 달라지는 것이죠. Long Context로 갈수록 이 효과가 더 커진다고 합니다. 그리고 가장 큰 차이는 첫 토큰에 대한 Attention에서 발생한다고 하네요.

따라서 문서 내 마스킹으로 Context Length를 줄이고 각 문서마다 위치 ID를 0으로 리셋하면 이 문제를 개선할 수 있지만 다양한 위치 ID에 대한 학습이 적어지죠. 이에 대해 레지스터 토큰을 사용하면 된다는 아이디어입니다. 결과적으로는 BoS 토큰을 쓰자는 것이죠.

딥 러닝 판은 저정밀도 연산에 워낙 익숙해서 대체로 간과되긴 하지만 (그리고 대체로 큰 문제가 없기도 하죠.) 가끔 수치 문제가 이렇게 기습할 때가 있습니다.

<english>
Problems of BFloat16 + RoPE. Contains a lot of analysis. I think this is the result from observations while tackling long context tasks.

The main point is that if we use RoPE with BFloat16 then effectiveness of RoPE as a relative positional encoding is decreased. That means attention values would vary a lot if we shift the positions. Longer context would increase this effect. And most difference is found on the first tokens.

So if we restrict context length with intra-document attention masking and reset position ids to 0 then this problem can be alleviated. But then training with various position ids is infeasible because context length of document would bound it. So this paper suggests to use register tokens, and that means we can introduct BoS tokens.

Low precision computations are so prevalent in the field of deep learning so it is commonly oerlooked, (and it is not problematic for most cases, anyway), but numerical precision problem sometimes ambush you.
</english>

#positional-encoding 