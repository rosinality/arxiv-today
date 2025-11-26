https://arxiv.org/abs/2511.20645

*PixelDiT: Pixel Diffusion Transformers for Image Generation* (Yongsheng Yu, Wei Xiong, Weili Nie, Yichen Sheng, Shiqiu Liu, Jiebo Luo)

> Latent-space modeling has been the standard for Diffusion Transformers (DiTs). However, it relies on a two-stage pipeline where the pretrained autoencoder introduces lossy reconstruction, leading to error accumulation while hindering joint optimization. To address these issues, we propose PixelDiT, a single-stage, end-to-end model that eliminates the need for the autoencoder and learns the diffusion process directly in the pixel space. PixelDiT adopts a fully transformer-based architecture shaped by a dual-level design: a patch-level DiT that captures global semantics and a pixel-level DiT that refines texture details, enabling efficient training of a pixel-space diffusion model while preserving fine details. Our analysis reveals that effective pixel-level token modeling is essential to the success of pixel diffusion. PixelDiT achieves 1.61 FID on ImageNet 256x256, surpassing existing pixel generative models by a large margin. We further extend PixelDiT to text-to-image generation and pretrain it at the 1024x1024 resolution in pixel space. It achieves 0.74 on GenEval and 83.5 on DPG-bench, approaching the best latent diffusion models.

픽셀 레벨 Diffusion은 그냥 되는 것일지도. 여기서는 픽셀과 좀 더 고레벨의 Semantic 경로를 나누는 구조를 사용 (https://arxiv.org/abs/2511.18822, https://arxiv.org/abs/2511.19365) (따라서 JiT가 여전히 가장 단순한 접근.)

Maybe pixel level diffusion is just works. This architecture uses dual stream of pixel and more higher, semantic pathways. (https://arxiv.org/abs/2511.18822, https://arxiv.org/abs/2511.19365) (Thus JiT is still simplest among this.)

#diffusion 