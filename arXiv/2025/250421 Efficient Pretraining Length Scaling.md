https://arxiv.org/abs/2504.14992

*Efficient Pretraining Length Scaling* (Bohong Wu, Shen Yan, Sijun Zhang, Jianqiao Lu, Yutao Zeng, Ya Wang, Xun Zhou)

> Recent advances in large language models have demonstrated the effectiveness of length scaling during post-training, yet its potential in pre-training remains underexplored. We present the Parallel Hidden Decoding Transformer (\textit{PHD}-Transformer), a novel framework that enables efficient length scaling during pre-training while maintaining inference efficiency. \textit{PHD}-Transformer achieves this through an innovative KV cache management strategy that distinguishes between original tokens and hidden decoding tokens. By retaining only the KV cache of original tokens for long-range dependencies while immediately discarding hidden decoding tokens after use, our approach maintains the same KV cache size as the vanilla transformer while enabling effective length scaling. To further enhance performance, we introduce two optimized variants: \textit{PHD-SWA} employs sliding window attention to preserve local dependencies, while \textit{PHD-CSWA} implements chunk-wise sliding window attention to eliminate linear growth in pre-filling time. Extensive experiments demonstrate consistent improvements across multiple benchmarks.

추론 CoT 같은 접근이 이젠 Length Scaling이라고 불리고 있군요. 프리트레이닝 시점에서 Length Scaling을 하려는 접근. 각 토큰을 복붙해서 K개로 증가시키고, 첫 토큰에 대해서만 KV 캐시에 저장, 나머지 토큰은 다음 토큰 예측에만 사용하는 방법입니다. 신박하긴 하네요.

<english>
Now approaches like reasoning CoT called as length scaling. A method for doing length scaling in pretraining. First increase number of each tokens by duplicating it K times, and only saves first token in KV cache, and use rest tokens for next token prediction. It's clever.
</english>

#pretraining 