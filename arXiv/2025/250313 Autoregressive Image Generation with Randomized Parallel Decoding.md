https://arxiv.org/abs/2503.10568

*Autoregressive Image Generation with Randomized Parallel Decoding* (Haopeng Li, Jinyue Yang, Guoqi Li, Huan Wang)

> We introduce ARPG, a novel visual autoregressive model that enables randomized parallel generation, addressing the inherent limitations of conventional raster-order approaches, which hinder inference efficiency and zero-shot generalization due to their sequential, predefined token generation order. Our key insight is that effective random-order modeling necessitates explicit guidance for determining the position of the next predicted token. To this end, we propose a novel guided decoding framework that decouples positional guidance from content representation, encoding them separately as queries and key-value pairs. By directly incorporating this guidance into the causal attention mechanism, our approach enables fully random-order training and generation, eliminating the need for bidirectional attention. Consequently, ARPG readily generalizes to zero-shot tasks such as image inpainting, outpainting, and resolution expansion. Furthermore, it supports parallel inference by concurrently processing multiple queries using a shared KV cache. On the ImageNet-1K 256 benchmark, our approach attains an FID of 1.94 with only 64 sampling steps, achieving over a 20-fold increase in throughput while reducing memory consumption by over 75% compared to representative recent autoregressive models at a similar scale.

Random order Autoregressive Image Generation. 이전 연구들이 위치 토큰을 더하거나 추가했다면 (https://arxiv.org/abs/2411.00776, https://arxiv.org/abs/2412.01827) 이쪽은 Cross Attention을 사용해서 위치 토큰을 Q로, 이미지 토큰을 KV로 사용한 형태네요.

디코더 내에서 Cross Attention을 사용한 구조는 이전에 등장했었죠. (https://arxiv.org/abs/2405.05254) 흥미롭네요.

Random order autoregressive image generation. While previous research added or appended positional tokens (https://arxiv.org/abs/2411.00776, https://arxiv.org/abs/2412.01827) this study adopted cross attention and used position tokens as Q, and image tokens as KV.

The use of cross attention within decoder has appeared before (https://arxiv.org/abs/2405.05254). Interesting.

#autoregressive-model #image-generation 