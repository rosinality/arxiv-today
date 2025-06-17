https://arxiv.org/abs/2410.08703

*On the token distance modeling ability of higher RoPE attention dimension* (Xiangyu Hong, Che Jiang, Biqing Qi, Fandong Meng, Mo Yu, Bowen Zhou, Jie Zhou)

> Length extrapolation algorithms based on Rotary position embedding (RoPE) have shown promising results in extending the context length of language models. However, understanding how position embedding can capture longer-range contextual information remains elusive. Based on the intuition that different dimensions correspond to different frequency of changes in RoPE encoding, we conducted a dimension-level analysis to investigate the correlation between a hidden dimension of an attention head and its contribution to capturing long-distance dependencies. Using our correlation metric, we identified a particular type of attention heads, which we named Positional Heads, from various length-extrapolated models. These heads exhibit a strong focus on long-range information interaction and play a pivotal role in long input processing, as evidence by our ablation. We further demonstrate the correlation between the efficiency of length extrapolation and the extension of the high-dimensional attention allocation of these heads. The identification of Positional Heads provides insights for future research in long-text comprehension.

토큰 사이의 거리 증가에 따라 RoPE의 저주파수 차원을 선호하는 헤드가 있고 이 헤드가 Long Context 문제에 대해서 중요하다는 아이디어. 저주파수 영역이 Semantic Attention의 기능을 한다는 분석과 (https://arxiv.org/abs/2410.06205) 결합해서 생각하는 것이 좋겠죠.

<english>
The idea that there are heads that prefers low frequency dimensions in RoPE regarding to increase of distance between tokens, and these heads are important to long context problems. I think it should be combined with analysis that low frequency dimens act as semantic attention. (https://arxiv.org/abs/2410.06205)
</english>

#positional-encoding #long-context

# Links

[[241008 Round and Round We Go! What makes Rotary Positional Encodings useful.md]]