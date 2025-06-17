https://arxiv.org/abs/2410.06205

*Round and Round We Go! What makes Rotary Positional Encodings useful?* (Federico Barbero, Alex Vitvitskyi, Christos Perivolaropoulos, Razvan Pascanu, Petar Veličković)

> Positional Encodings (PEs) are a critical component of Transformer-based Large Language Models (LLMs), providing the attention mechanism with important sequence-position information. One of the most popular types of encoding used today in LLMs are Rotary Positional Encodings (RoPE), that rotate the queries and keys based on their relative distance. A common belief is that RoPE is useful because it helps to decay token dependency as relative distance increases. In this work, we argue that this is unlikely to be the core reason. We study the internals of a trained Gemma 7B model to understand how RoPE is being used at a mechanical level. We find that Gemma learns to use RoPE to construct robust "positional" attention patterns by exploiting the highest frequencies. We also find that, in general, Gemma greatly prefers to use the lowest frequencies of RoPE, which we suspect are used to carry semantic information. We mathematically prove interesting behaviours of RoPE and conduct experiments to verify our findings, proposing a modification of RoPE that fixes some highlighted issues and improves performance. We believe that this work represents an interesting step in better understanding PEs in LLMs, which we believe holds crucial value for scaling LLMs to large sizes and context lengths.

RoPE에서 고주파수 차원들은 위치 기반 Attention에 사용되고 저주파수 차원들은 의미 기반 Attention에 사용된다는 발견. 저주파수 차원들이 토큰 위치에 따른 변화가 적기에 의미 기반 Attention에 사용되는 것일 텐데, 그렇다면 저주파수 차원이 없는 쪽이 더 나을 수도 있겠죠.

그래서 부분적으로만 RoPE를 적용하는 실험을 했습니다. 사실 RoPE에 본래 있었던 옵션이기도 하죠. Long Context에서의 특성은 어떨지도 궁금하네요.

<english>
Discovery of high frequency dimensions of RoPE is used in position based attention, and low frequency dimensions is used for semantic attention. It is because of there are less change in low frequency dimensions along with token positions, and then it could better with no low frequency dimensions at all.

So they did experiment that only partially applying RoPE. Actually it was an option in original RoPE. I wonder the characteristics in long context.
</english>

#positional-encoding