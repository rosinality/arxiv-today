https://arxiv.org/abs/2410.02367

*SageAttention: Accurate 8-Bit Attention for Plug-and-play Inference Acceleration* (Jintao Zhang, Jia wei, Pengle Zhang, Jun Zhu, Jianfei Chen)

> The transformer architecture predominates across various models. As the heart of the transformer, attention has a computational complexity of O(N^2), compared to O(N) for linear transformations. When handling large sequence lengths, attention becomes the primary time-consuming component. Although quantization has proven to be an effective method for accelerating model inference, existing quantization methods primarily focus on optimizing the linear layer. In response, we first analyze the feasibility of quantization in attention detailedly. Following that, we propose SageAttention, a highly efficient and accurate quantization method for attention. The OPS (operations per second) of our approach outperforms FlashAttention2 and xformers by about 2.1 times and 2.7 times, respectively. SageAttention also achieves superior accuracy performance over FlashAttention3. Comprehensive experiments confirm that our approach incurs almost no end-to-end metrics loss across diverse models, including those for large language processing, image generation, and video generation.

8 Bit Flash Attention. Quantized Flash Attention의 구현은 이전에도 있었는데 (https://arxiv.org/abs/2409.16997) 이쪽은 어떻게 Quantization을 해야할 것인가에 대해서 탐색을 많이 했네요.

<english>
8 Bit Flash Attention. Quantized Flash Attention was came out previously (https://arxiv.org/abs/2409.16997) But this study explored further for how we should do quantization.
</english>

#efficiency

# Links

