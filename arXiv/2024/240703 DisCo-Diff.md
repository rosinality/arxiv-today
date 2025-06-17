https://arxiv.org/abs/2407.03300

*DisCo-Diff: Enhancing Continuous Diffusion Models with Discrete Latents* (Yilun Xu, Gabriele Corso, Tommi Jaakkola, Arash Vahdat, Karsten Kreis)

> Diffusion models (DMs) have revolutionized generative learning. They utilize a diffusion process to encode data into a simple Gaussian distribution. However, encoding a complex, potentially multimodal data distribution into a single continuous Gaussian distribution arguably represents an unnecessarily challenging learning problem. We propose Discrete-Continuous Latent Variable Diffusion Models (DisCo-Diff) to simplify this task by introducing complementary discrete latent variables. We augment DMs with learnable discrete latents, inferred with an encoder, and train DM and encoder end-to-end. DisCo-Diff does not rely on pre-trained networks, making the framework universally applicable. The discrete latents significantly simplify learning the DM's complex noise-to-data mapping by reducing the curvature of the DM's generative ODE. An additional autoregressive transformer models the distribution of the discrete latents, a simple step because DisCo-Diff requires only few discrete variables with small codebooks. We validate DisCo-Diff on toy data, several image synthesis tasks as well as molecular docking, and find that introducing discrete latents consistently improves model performance. For example, DisCo-Diff achieves state-of-the-art FID scores on class-conditioned ImageNet-64/128 datasets with ODE sampler.

Diffusion 모델로 Unimodal 가우시안 분포에서 모드가 여럿이고 분리된 컴포넌트로 구성된 이미지 분포로 매핑하는 것은 매핑을 굉장히 복잡하게 만든다는 아이디어. 이에 대해 컨디션 정보를 추가하는 방법을 사용했습니다. 이미지 입력을 Discrete Code로 바꾸고 Denoising 모델에 추가 정보로 제공하고, 이 Discrete Code는 Autoregressive 모델을 사용해 생성하는 거죠.

단순한 코드로 이미지 분포의 복잡성을 대응하기 위해 특정한 클래스 레이블을 넘어선 컨디션 정보를 이미지에서 추정해 사용한다는 아이디어는 굉장히 예전에 GAN에서 등장했던 아이디어이기도 합니다. (https://arxiv.org/abs/2006.06500, https://arxiv.org/abs/2006.10728, https://arxiv.org/abs/2012.02162) 이렇게 다시 보게 되니 반갑네요.

#diffusion #autoregressive-model

# Links

[[200611 Rethinking the Truly Unsupervised Image-to-Image Translation.md]]
[[201203 Self-labeled Conditional GANs.md]]
[[200618 Diverse Image Generation via Self-Conditioned GANs.md]]