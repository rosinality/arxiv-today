https://arxiv.org/abs/2405.05967

*Distilling Diffusion Models into Conditional GANs* (Minguk Kang, Richard Zhang, Connelly Barnes, Sylvain Paris, Suha Kwak, Jaesik Park, Eli Shechtman, Jun-Yan Zhu, Taesung Park)

> We propose a method to distill a complex multistep diffusion model into a single-step conditional GAN student model, dramatically accelerating inference, while preserving image quality. Our approach interprets diffusion distillation as a paired image-to-image translation task, using noise-to-image pairs of the diffusion model's ODE trajectory. For efficient regression loss computation, we propose E-LatentLPIPS, a perceptual loss operating directly in diffusion model's latent space, utilizing an ensemble of augmentations. Furthermore, we adapt a diffusion model to construct a multi-scale discriminator with a text alignment loss to build an effective conditional GAN-based formulation. E-LatentLPIPS converges more efficiently than many existing distillation methods, even accounting for dataset construction costs. We demonstrate that our one-step generator outperforms cutting-edge one-step diffusion distillation models - DMD, SDXL-Turbo, and SDXL-Lightning - on the zero-shot COCO benchmark.

Diffusion 모델의 샘플을 사용해 노이즈와 이미지의 페어를 만들고 이걸 Img2Img로 생각해서 학습시켰군요. 이 문제에 대해 LPIPS 같은 Perceptual Metric이 효과적인데 Latent Diffusion이니 Latent에 대해 동작하는 Latent LPIPS에 GAN Discriminator를 사용했습니다. 재미있네요.

#diffusion #efficiency #distillation 