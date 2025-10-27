https://arxiv.org/abs/2510.15301

*Latent Diffusion Model without Variational Autoencoder* (Minglei Shi, Haolin Wang, Wenzhao Zheng, Ziyang Yuan, Xiaoshi Wu, Xintao Wang, Pengfei Wan, Jie Zhou, Jiwen Lu)

> Recent progress in diffusion-based visual generation has largely relied on latent diffusion models with variational autoencoders (VAEs). While effective for high-fidelity synthesis, this VAE+diffusion paradigm suffers from limited training efficiency, slow inference, and poor transferability to broader vision tasks. These issues stem from a key limitation of VAE latent spaces: the lack of clear semantic separation and strong discriminative structure. Our analysis confirms that these properties are crucial not only for perception and understanding tasks, but also for the stable and efficient training of latent diffusion models. Motivated by this insight, we introduce SVG, a novel latent diffusion model without variational autoencoders, which leverages self-supervised representations for visual generation. SVG constructs a feature space with clear semantic discriminability by leveraging frozen DINO features, while a lightweight residual branch captures fine-grained details for high-fidelity reconstruction. Diffusion models are trained directly on this semantically structured latent space to facilitate more efficient learning. As a result, SVG enables accelerated diffusion training, supports few-step sampling, and improves generative quality. Experimental results further show that SVG preserves the semantic and discriminative capabilities of the underlying self-supervised representations, providing a principled pathway toward task-general, high-quality visual representations.

RAE에 대한 개선은 이미 등장. Residual Encoder로 이미지 토큰의 Recon 퀄리티를 향상.

Improvements on RAE is already released. Using residual encoder to enhance reconstruction quality of image tokens.

#diffusion #tokenizer 