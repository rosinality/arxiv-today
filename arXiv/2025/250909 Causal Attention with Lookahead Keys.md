https://arxiv.org/abs/2509.07301

*Causal Attention with Lookahead Keys* (Zhuoqing Song, Peng Sun, Huizhuo Yuan, Quanquan Gu)

> In standard causal attention, each token's query, key, and value (QKV) are static and encode only preceding context. We introduce CAuSal aTtention with Lookahead kEys (CASTLE), an attention mechanism that continually updates each token's keys as the context unfolds. We term these updated keys lookahead keys because they belong to earlier positions yet integrate information from tokens that appear later relative to those positions, while strictly preserving the autoregressive property. Although the mechanism appears sequential, we derive a mathematical equivalence that avoids explicitly materializing lookahead keys at each position and enables efficient parallel training. On language modeling benchmarks, CASTLE consistently outperforms standard causal attention across model scales, reducing validation perplexity and improving performance on a range of downstream tasks.

Autoregressive 생성 과정에서 이전 키들을 이후 토큰을 사용해 업데이트. 이후 토큰들에 대한 정보가 포함된 키들을(Lookahead Keys) 따로 사용해서 구현.

Updates keys using later tokens during autoregressive generation. Implemented by using a separate set of keys that contains information from later tokens (lookahead keys).

#attention #transformer 