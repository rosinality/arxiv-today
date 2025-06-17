https://arxiv.org/abs/2502.14831

*Improving the Diffusability of Autoencoders* (Ivan Skorokhodov, Sharath Girish, Benran Hu, Willi Menapace, Yanyu Li, Rameen Abdal, Sergey Tulyakov, Aliaksandr Siarohin)

> Latent diffusion models have emerged as the leading approach for generating high-quality images and videos, utilizing compressed latent representations to reduce the computational burden of the diffusion process. While recent advancements have primarily focused on scaling diffusion backbones and improving autoencoder reconstruction quality, the interaction between these components has received comparatively less attention. In this work, we perform a spectral analysis of modern autoencoders and identify inordinate high-frequency components in their latent spaces, which are especially pronounced in the autoencoders with a large bottleneck channel size. We hypothesize that this high-frequency component interferes with the coarse-to-fine nature of the diffusion synthesis process and hinders the generation quality. To mitigate the issue, we propose scale equivariance: a simple regularization strategy that aligns latent and RGB spaces across frequencies by enforcing scale equivariance in the decoder. It requires minimal code changes and only up to 20K autoencoder fine-tuning steps, yet significantly improves generation quality, reducing FID by 19% for image generation on ImageNet-1K 256x256 and FVD by at least 44% for video generation on Kinetics-700 17x256x256.

VAE 토크나이저의 Latent에 고주파수 성분이 많이 포함되어 있고 이것이 Diffusion 학습에 문제가 될 수 있다는 분석. GAN 시절의 분석들이 생각나는군요. (https://arxiv.org/abs/2106.12423)

<english>
The analysis on VAE tokenizers that it has relatively large amount high-frequency components and it can hinder diffusion trainings. It reminds me the analysis in GAN-era. (https://arxiv.org/abs/2106.12423)
</english>

#diffusion #tokenizer 