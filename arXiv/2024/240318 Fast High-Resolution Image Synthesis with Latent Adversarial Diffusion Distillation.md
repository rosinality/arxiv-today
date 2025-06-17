https://arxiv.org/abs/2403.12015

*Fast High-Resolution Image Synthesis with Latent Adversarial Diffusion Distillation* (Axel Sauer, Frederic Boesel, Tim Dockhorn, Andreas Blattmann, Patrick Esser, Robin Rombach)

> Diffusion models are the main driver of progress in image and video synthesis, but suffer from slow inference speed. Distillation methods, like the recently introduced adversarial diffusion distillation (ADD) aim to shift the model from many-shot to single-step inference, albeit at the cost of expensive and difficult optimization due to its reliance on a fixed pretrained DINOv2 discriminator. We introduce Latent Adversarial Diffusion Distillation (LADD), a novel distillation approach overcoming the limitations of ADD. In contrast to pixel-based ADD, LADD utilizes generative features from pretrained latent diffusion models. This approach simplifies training and enhances performance, enabling high-resolution multi-aspect ratio image synthesis. We apply LADD to Stable Diffusion 3 (8B) to obtain SD3-Turbo, a fast model that matches the performance of state-of-the-art text-to-image generators using only four unguided sampling steps. Moreover, we systematically investigate its scaling behavior and demonstrate LADD's effectiveness in various applications such as image editing and inpainting.

이미지 대신 Latent에 대해서 Adversarial Distillation. (https://arxiv.org/abs/2311.17042) 거기에 Teacher Diffusion 모델의 Feature를 사용해 Projected GAN을 적용해서 세팅을 더 단순하게 만들었습니다.

#diffusion #distillation

# Links

[[231128 Adversarial Diffusion Distillation.md]]