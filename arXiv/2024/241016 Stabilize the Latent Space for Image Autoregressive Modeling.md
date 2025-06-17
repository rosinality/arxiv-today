https://arxiv.org/abs/2410.12490

*Stabilize the Latent Space for Image Autoregressive Modeling: A Unified Perspective* (Yongxin Zhu, Bocheng Li, Hang Zhang, Xin Li, Linli Xu, Lidong Bing)

> Latent-based image generative models, such as Latent Diffusion Models (LDMs) and Mask Image Models (MIMs), have achieved notable success in image generation tasks. These models typically leverage reconstructive autoencoders like VQGAN or VAE to encode pixels into a more compact latent space and learn the data distribution in the latent space instead of directly from pixels. However, this practice raises a pertinent question: Is it truly the optimal choice? In response, we begin with an intriguing observation: despite sharing the same latent space, autoregressive models significantly lag behind LDMs and MIMs in image generation. This finding contrasts sharply with the field of NLP, where the autoregressive model GPT has established a commanding presence. To address this discrepancy, we introduce a unified perspective on the relationship between latent space and generative models, emphasizing the stability of latent space in image generative modeling. Furthermore, we propose a simple but effective discrete image tokenizer to stabilize the latent space for image generative modeling. Experimental results show that image autoregressive modeling with our tokenizer (DiGIT) benefits both image understanding and image generation with the next token prediction principle, which is inherently straightforward for GPT models but challenging for other generative models. Remarkably, for the first time, a GPT-style autoregressive model for images outperforms LDMs, which also exhibits substantial improvement akin to GPT when scaling up model size. Our findings underscore the potential of an optimized latent space and the integration of discrete tokenization in advancing the capabilities of image generative models. The code is available at \url{https://github.com/DAMO-NLP-SG/DiGIT}.

Reconstruction으로 학습한 VQ 토큰이 생성에는 적합하지 않을 수 있다는 아이디어. 그래서 SSL로 학습한 인코더의 Feature에 대해 K-Means로 토큰을 뽑는 방법을 사용했습니다. 비슷한 연구들이 이전에도 나왔었죠. (https://arxiv.org/abs/2406.11837, https://arxiv.org/abs/2407.09087)

이런 형태의 2단계 학습은 단계 사이에서 학습 시그널이 전달되지 않기 때문에 기본적인 문제가 있죠. 그리고 학습하는 것은 학습하지 않는 것보다 낫죠.

<english>
Idea that VQ token learnt using reconstruction may be not appropriate for generation. So they have used SSL encoder and extract tokens using K-means on the image features. Similar researches has came out earlier. (https://arxiv.org/abs/2406.11837, https://arxiv.org/abs/2407.09087)

Inherent problem in these two stage training is that training signal is not transferred between the stages. And make it learning is better than not learning it.
</english>

#vq #autoregressive-model

# Links

[[240617 Scaling the Codebook Size of VQGAN to 100,000 with a Utilization Rate of 99%.md]]
[[240712 On the Role of Discrete Tokenization in Visual Representation Learning.md]]