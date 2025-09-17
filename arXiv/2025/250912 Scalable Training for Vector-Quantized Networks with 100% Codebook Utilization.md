https://arxiv.org/abs/2509.10140

*Scalable Training for Vector-Quantized Networks with 100% Codebook Utilization* (Yifan Chang, Jie Qin, Limeng Qiao, Xiaofeng Wang, Zheng Zhu, Lin Ma, Xingang Wang)

> Vector quantization (VQ) is a key component in discrete tokenizers for image generation, but its training is often unstable due to straight-through estimation bias, one-step-behind updates, and sparse codebook gradients, which lead to suboptimal reconstruction performance and low codebook usage. In this work, we analyze these fundamental challenges and provide a simple yet effective solution. To maintain high codebook usage in VQ networks (VQN) during learning annealing and codebook size expansion, we propose VQBridge, a robust, scalable, and efficient projector based on the map function method. VQBridge optimizes code vectors through a compress-process-recover pipeline, enabling stable and effective codebook training. By combining VQBridge with learning annealing, our VQN achieves full (100%) codebook usage across diverse codebook configurations, which we refer to as FVQ (FullVQ). Through extensive experiments, we demonstrate that FVQ is effective, scalable, and generalizable: it attains 100% codebook usage even with a 262k-codebook, achieves state-of-the-art reconstruction performance, consistently improves with larger codebooks, higher vector channels, or longer training, and remains effective across different VQ variants. Moreover, when integrated with LlamaGen, FVQ significantly enhances image generation performance, surpassing visual autoregressive models (VAR) by 0.5 and diffusion models (DiT) by 0.2 rFID, highlighting the importance of high-quality tokenizers for strong autoregressive image generation.

Projection을 사용해 코드북 Collapse를 방지. Linear로는 약하다는 것을 발견해서 ViT를 사용.

Prevents codebook collapse using projection (https://arxiv.org/abs/2411.02038). They found that linear mapping is not strong enough, thus employed ViT for this.

#vq #tokenizer 