https://arxiv.org/abs/2412.03069

*TokenFlow: Unified Image Tokenizer for Multimodal Understanding and Generation* (Liao Qu, Huichao Zhang, Yiheng Liu, Xu Wang, Yi Jiang, Yiming Gao, Hu Ye, Daniel K. Du, Zehuan Yuan, Xinglong Wu)

> We present TokenFlow, a novel unified image tokenizer that bridges the long-standing gap between multimodal understanding and generation. Prior research attempt to employ a single reconstruction-targeted Vector Quantization (VQ) encoder for unifying these two tasks. We observe that understanding and generation require fundamentally different granularities of visual information. This leads to a critical trade-off, particularly compromising performance in multimodal understanding tasks. TokenFlow addresses this challenge through an innovative dual-codebook architecture that decouples semantic and pixel-level feature learning while maintaining their alignment via a shared mapping mechanism. This design enables direct access to both high-level semantic representations crucial for understanding tasks and fine-grained visual features essential for generation through shared indices. Our extensive experiments demonstrate TokenFlow's superiority across multiple dimensions. Leveraging TokenFlow, we demonstrate for the first time that discrete visual input can surpass LLaVA-1.5 13B in understanding performance, achieving a 7.2\% average improvement. For image reconstruction, we achieve a strong FID score of 0.63 at 384*384 resolution. Moreover, TokenFlow establishes state-of-the-art performance in autoregressive image generation with a GenEval score of 0.55 at 256*256 resolution, achieving comparable results to SDXL.

인식과 생성을 동시에 추구하는 이미지 토크나이저. 시맨틱 인코더와 픽셀 인코더를 두고, 각 인코더로 인코딩된 Feature와의 거리의 가중합으로 가장 가까운 코드를 찾는 방식입니다. 그리고 시맨틱 디코더를 추가로 사용해서 BEiT v2 Feature와의 차이를 Loss로 사용했군요. (https://arxiv.org/abs/2208.06366)

<english>
An image tokenizer that pursues both recognition and generation. They used semantic and pixel encoder, and they select nearest code with weight sum of distances between each features and codes. And they also used semantic decoder and used a loss between the difference with the features from BEiT v2.
</english>

#vq #image-generation #image-text

# Links

[[220812 BEiT v2.md]]