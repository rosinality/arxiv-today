https://arxiv.org/abs/2312.02696

Analyzing and Improving the Training Dynamics of Diffusion Models (Tero Karras, Miika Aittala, Jaakko Lehtinen, Janne Hellsten, Timo Aila, Samuli Laine)

오랜만에 Tero Karras의 논문을 보네요. 학습의 불안정성을 해소하기 위해 아키텍처를 갈아 엎고, activation 크기의 증가를 억제하기 위해 Weight Normalization을 도입했습니다. Weight Normalization도 정말 오랜만에 봅니다.

Weight Normalization을 도입하니 weight가 커지는 경향이 있어서 강제로 weight를 normalize 하는 것과 함께 learning rate schedule을 조절하고 group normalization을 날린 후 pixel normalization을 끼워넣고 scaling layer를 추가했네요. 이렇게 모델을 깎고 깎아 ImageNet-512 FID SOTA를 찍었습니다.

StyleGAN 시절에도 느꼈던 것이지만 모델을 분석하고 개선하는 것에 타의 추종을 불허하는군요. 이렇게 보면 이미 뻔하고 뻔한 아키텍처라고 해도 학습 동역학을 깊게 이해한다면 개선할 수 있는 여지가 많다는 생각이 들죠. 트랜스포머 LM을 깎아볼 생각은 없을지 궁금하네요.

#diffusion 

[[200122 StyleGAN 2]]