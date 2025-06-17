https://arxiv.org/abs/2410.11081

*Simplifying, Stabilizing and Scaling Continuous-Time Consistency Models* (Cheng Lu, Yang Song)

> Consistency models (CMs) are a powerful class of diffusion-based generative models optimized for fast sampling. Most existing CMs are trained using discretized timesteps, which introduce additional hyperparameters and are prone to discretization errors. While continuous-time formulations can mitigate these issues, their success has been limited by training instability. To address this, we propose a simplified theoretical framework that unifies previous parameterizations of diffusion models and CMs, identifying the root causes of instability. Based on this analysis, we introduce key improvements in diffusion process parameterization, network architecture, and training objectives. These changes enable us to train continuous-time CMs at an unprecedented scale, reaching 1.5B parameters on ImageNet 512x512. Our proposed training algorithm, using only two sampling steps, achieves FID scores of 2.06 on CIFAR-10, 1.48 on ImageNet 64x64, and 1.88 on ImageNet 512x512, narrowing the gap in FID scores with the best existing diffusion models to within 10%.

Continuous-Time Consistency Model에 대한 학습 안정성 개선. 이쪽은 Consistency Model에 대한 개선 작업을 계속하고 있군요.

<english>
Improvements on training stability of continuous-time consistency models. Authors continuously doing the work for improving consistency models.
</english>

#diffusion 