https://arxiv.org/abs/2410.17980

*Stick-breaking Attention* (Shawn Tan, Yikang Shen, Songlin Yang, Aaron Courville, Rameswar Panda)

> The self-attention mechanism traditionally relies on the softmax operator, necessitating positional embeddings like RoPE, or position biases to account for token order. But current methods using still face length generalisation challenges. We propose an alternative attention mechanism based on the stick-breaking process: For each token before the current, we determine a break point $\beta_{i,j}$, which represents the proportion of the remaining stick to allocate to the current token. We repeat the process until the stick is fully allocated, resulting in a sequence of attention weights. This process naturally incorporates recency bias, which has linguistic motivations for grammar parsing (Shen et. al., 2017). We study the implications of replacing the conventional softmax-based attention mechanism with stick-breaking attention. We then discuss implementation of numerically stable stick-breaking attention and adapt Flash Attention to accommodate this mechanism. When used as a drop-in replacement for current softmax+RoPE attention systems, we find that stick-breaking attention performs competitively with current methods on length generalisation and downstream tasks. Stick-breaking also performs well at length generalisation, allowing a model trained with $2^{11}$ context window to perform well at $2^{14}$ with perplexity improvements.

Stick Breaking Attention에 대한 (https://arxiv.org/abs/2306.04640) 효율적인 구현이 등장했군요. Stick Breaking Attention은 특정 시점에서 Attention Weight가 높은 토큰이 있다면 그 이전 토큰들의 Attention Weight를 억제하는 형태죠. 다만 멀리 떨어진 토큰에 대해서 지나치게 억제될 가능성이 있지 않을까 싶네요.

<english>
Efficient implementation for stick breaking attention. (https://arxiv.org/abs/2306.04640) Stick breaking attention suppresses attention weights to previous tokens if there are tokens with high attention weight between that tokens and current tokens. But I suspect it could suppress too much for tokens with far distances.
</english>

#attention #positional-encoding

# Links

