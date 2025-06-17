https://arxiv.org/abs/2403.06807

*Multistep Consistency Models* (Jonathan Heek, Emiel Hoogeboom, Tim Salimans)

> Diffusion models are relatively easy to train but require many steps to generate samples. Consistency models are far more difficult to train, but generate samples in a single step. In this paper we propose Multistep Consistency Models: A unification between Consistency Models (Song et al., 2023) and TRACT (Berthelot et al., 2023) that can interpolate between a consistency model and a diffusion model: a trade-off between sampling speed and sampling quality. Specifically, a 1-step consistency model is a conventional consistency model whereas we show that a $\infty$-step consistency model is a diffusion model. Multistep Consistency Models work really well in practice. By increasing the sample budget from a single step to 2-8 steps, we can train models more easily that generate higher quality samples, while retaining much of the sampling speed benefits. Notable results are 1.4 FID on Imagenet 64 in 8 step and 2.1 FID on Imagenet128 in 8 steps with consistency distillation. We also show that our method scales to a text-to-image diffusion model, generating samples that are very close to the quality of the original model.

Consistency Models를 스텝 0 뿐만 아니라 중간 스텝을 예측할 수 있도록 수정한 방법. 이 스텝의 수가 전체 스텝 수와 일치하게 되면 Diffusion과 동일해집니다. 추가로 Deterministic Sampler에서 오차에 의해 발생하는 지나치게 스무딩된 샘플을 추정한 노이즈의 비중을 높이는 방식으로 개선했습니다. (aDDIM) 8 스텝 정도로 ImageNet에서 SOTA 성능을 내고 있네요.

추가로 구글에서 20B 규모 Text2Image 모델을 만들었다는 것을 귀띔하고 있군요.

#diffusion 