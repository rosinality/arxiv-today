https://arxiv.org/abs/2503.07565

*Inductive Moment Matching* (Linqi Zhou, Stefano Ermon, Jiaming Song)

> Diffusion models and Flow Matching generate high-quality samples but are slow at inference, and distilling them into few-step models often leads to instability and extensive tuning. To resolve these trade-offs, we propose Inductive Moment Matching (IMM), a new class of generative models for one- or few-step sampling with a single-stage training procedure. Unlike distillation, IMM does not require pre-training initialization and optimization of two networks; and unlike Consistency Models, IMM guarantees distribution-level convergence and remains stable under various hyperparameters and standard model architectures. IMM surpasses diffusion models on ImageNet-256x256 with 1.99 FID using only 8 inference steps and achieves state-of-the-art 2-step FID of 1.98 on CIFAR-10 for a model trained from scratch.

1 or Few-step Single Stage 이미지 생성 모델. s < r < t 시점을 가정할 때 r 시점의 샘플에서 예측한 s 시점의 분포와 t 시점에서 예측한 분포를 MMD로 일치시키는 방법입니다. Consistency Model의 확장으로서 생각할 수 있을 것 같네요. 굉장히 흥미로운 결과입니다.

<english>
1 or few shot image generation method with single stage training. The method is when assume s < r < t times, match distribution of time s generated from samples at r and t using MMD. It would be generalization of consistency models. It is very intruging results.
</english>

#diffusion 