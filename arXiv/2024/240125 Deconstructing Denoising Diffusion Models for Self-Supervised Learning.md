https://arxiv.org/abs/2401.14404

*Deconstructing Denoising Diffusion Models for Self-Supervised Learning* (Xinlei Chen, Zhuang Liu, Saining Xie, Kaiming He)

> In this study, we examine the representation learning abilities of Denoising Diffusion Models (DDM) that were originally purposed for image generation. Our philosophy is to deconstruct a DDM, gradually transforming it into a classical Denoising Autoencoder (DAE). This deconstructive procedure allows us to explore how various components of modern DDMs influence self-supervised representation learning. We observe that only a very few modern components are critical for learning good representations, while many others are nonessential. Our study ultimately arrives at an approach that is highly simplified and to a large extent resembles a classical DAE. We hope our study will rekindle interest in a family of classical methods within the realm of modern self-supervised learning.

Diffusion Model을 변형해 Denoising Auto Encoder와 비슷하게 맞추면서 Self Supervision에 특화시키기. 픽셀 단위의 노이즈는 충분하지 않은 듯 하나 VAE를 쓸 필요는 없어서 PCA로 축소한 다음 노이즈를 걸고 Inverse PCA로 복원한 이미지를 입력으로 쓰는 방식을 택했습니다. 그 입력에 대해 원본 이미지를 Reconstruction 하는 것을 학습 타겟으로 만들었네요. 생성을 위한 노이즈 스케쥴 등도 빼버렸습니다.

생성과 Self Supervision 사이의 갭에 대해 생각해보게 되네요. 이 갭을 줄이거나 없애는 것이 흥미로운 목표겠죠.

#diffusion #self-supervision 