https://arxiv.org/abs/2502.09609

*Score-of-Mixture Training: Training One-Step Generative Models Made Simple* (Tejas Jayashankar, J. Jon Ryu, Gregory Wornell)

> We propose Score-of-Mixture Training (SMT), a novel framework for training one-step generative models by minimizing a class of divergences called the $\alpha$-skew Jensen-Shannon divergence. At its core, SMT estimates the score of mixture distributions between real and fake samples across multiple noise levels. Similar to consistency models, our approach supports both training from scratch (SMT) and distillation using a pretrained diffusion model, which we call Score-of-Mixture Distillation (SMD). It is simple to implement, requires minimal hyperparameter tuning, and ensures stable training. Experiments on CIFAR-10 and ImageNet 64x64 show that SMT/SMD are competitive with and can even outperform existing methods.

Forward와 Reverse KL을 Interpolate하는 Divergence를 Objective로 하여 학습. 이 Objective에 대한 학습을 위해서는 Score Model을 사용.

<english>
Training on-step generative models using divergence interpolates forward and reverse Kl as an objective. To train a model with this objective amortized score model is used.
</english>

#image-generation #diffusion #gan 