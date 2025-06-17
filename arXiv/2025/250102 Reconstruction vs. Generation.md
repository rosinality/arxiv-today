https://arxiv.org/abs/2501.01423

*Reconstruction vs. Generation: Taming Optimization Dilemma in Latent Diffusion Models* (Jingfeng Yao, Xinggang Wang)

> Latent diffusion models with Transformer architectures excel at generating high-fidelity images. However, recent studies reveal an optimization dilemma in this two-stage design: while increasing the per-token feature dimension in visual tokenizers improves reconstruction quality, it requires substantially larger diffusion models and more training iterations to achieve comparable generation performance. Consequently, existing systems often settle for sub-optimal solutions, either producing visual artifacts due to information loss within tokenizers or failing to converge fully due to expensive computation costs. We argue that this dilemma stems from the inherent difficulty in learning unconstrained high-dimensional latent spaces. To address this, we propose aligning the latent space with pre-trained vision foundation models when training the visual tokenizers. Our proposed VA-VAE (Vision foundation model Aligned Variational AutoEncoder) significantly expands the reconstruction-generation frontier of latent diffusion models, enabling faster convergence of Diffusion Transformers (DiT) in high-dimensional latent spaces. To exploit the full potential of VA-VAE, we build an enhanced DiT baseline with improved training strategies and architecture designs, termed LightningDiT. The integrated system achieves state-of-the-art (SOTA) performance on ImageNet 256x256 generation with an FID score of 1.35 while demonstrating remarkable training efficiency by reaching an FID score of 2.11 in just 64 epochs--representing an over 21 times convergence speedup compared to the original DiT. Models and codes are available at: https://github.com/hustvl/LightningDiT.

VAE의 차원을 증가시켜 Reconstruction 성능을 높였을 때 Generation 모델을 학습시키는 것이 어려워지는 문제에 대한 해결. VAE의 인코딩 결과에 이미지 백본의 출력으로 제약을 걸어 학습을 쉽게 만든다는 아이디어. 요즘 많이 나오는 문제 의식이죠. (https://arxiv.org/abs/2412.16326, https://arxiv.org/abs/2412.03069)

본질적으로는 VAE와 Diffusion의 학습이 분리되어 있다는 것이 문제이긴 하겠습니다.

<english>
Solving the problem of it is harder to train generation model when we enhances reconstruction performances by incresing the dimensions of VAE. The idea is make it easy to train on by induces a restriction on encoded features from VAE by using the outputs of image backbones. It is frequently appearing line of researches these days (https://arxiv.org/abs/2412.16326, https://arxiv.org/abs/2412.03069).

Essentially it is the problem rooted in the separation of VAE and diffusion training.
</english>

#vq #vae #diffusion

# Links

[[241220 When Worse is Better.md]]
[[241204 TokenFlow.md]]