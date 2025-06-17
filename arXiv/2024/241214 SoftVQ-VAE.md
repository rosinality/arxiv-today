https://arxiv.org/abs/2412.10958

*SoftVQ-VAE: Efficient 1-Dimensional Continuous Tokenizer* (Hao Chen, Ze Wang, Xiang Li, Ximeng Sun, Fangyi Chen, Jiang Liu, Jindong Wang, Bhiksha Raj, Zicheng Liu, Emad Barsoum)

> Efficient image tokenization with high compression ratios remains a critical challenge for training generative models. We present SoftVQ-VAE, a continuous image tokenizer that leverages soft categorical posteriors to aggregate multiple codewords into each latent token, substantially increasing the representation capacity of the latent space. When applied to Transformer-based architectures, our approach compresses 256x256 and 512x512 images using as few as 32 or 64 1-dimensional tokens. Not only does SoftVQ-VAE show consistent and high-quality reconstruction, more importantly, it also achieves state-of-the-art and significantly faster image generation results across different denoising-based generative models. Remarkably, SoftVQ-VAE improves inference throughput by up to 18x for generating 256x256 images and 55x for 512x512 images while achieving competitive FID scores of 1.78 and 2.21 for SiT-XL. It also improves the training efficiency of the generative models by reducing the number of training iterations by 2.3x while maintaining comparable performance. With its fully-differentiable design and semantic-rich latent space, our experiment demonstrates that SoftVQ-VQE achieves efficient tokenization without compromising generation quality, paving the way for more efficient generative models. Code and model are released.

Semantic Token과 비슷한 Latent Token에 더해 코드북에 대한 Weighted sum으로 이미지 토큰을 추출. 추가적으로 이미지 Feature에 대한 Loss를 걸어줬군요. (https://arxiv.org/abs/2406.07550, https://arxiv.org/abs/2412.03069)

<english>
Extract image tokens using latent tokens similar to semantic token and weighted sum of codebooks by distance of token and it. Additionally they used loss against pretrained image features. (https://arxiv.org/abs/2406.07550, https://arxiv.org/abs/2412.03069)
</english>

#tokenizer #image-generation

# Links

[[240611 An Image is Worth 32 Tokens for Reconstruction and Generation.md]]
[[241204 TokenFlow.md]]