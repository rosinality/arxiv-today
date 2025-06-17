https://arxiv.org/abs/2410.18958

*Stable Consistency Tuning: Understanding and Improving Consistency Models* (Fu-Yun Wang, Zhengyang Geng, Hongsheng Li)

> Diffusion models achieve superior generation quality but suffer from slow generation speed due to the iterative nature of denoising. In contrast, consistency models, a new generative family, achieve competitive performance with significantly faster sampling. These models are trained either through consistency distillation, which leverages pretrained diffusion models, or consistency training/tuning directly from raw data. In this work, we propose a novel framework for understanding consistency models by modeling the denoising process of the diffusion model as a Markov Decision Process (MDP) and framing consistency model training as the value estimation through Temporal Difference~(TD) Learning. More importantly, this framework allows us to analyze the limitations of current consistency training/tuning strategies. Built upon Easy Consistency Tuning (ECT), we propose Stable Consistency Tuning (SCT), which incorporates variance-reduced learning using the score identity. SCT leads to significant performance improvements on benchmarks such as CIFAR-10 and ImageNet-64. On ImageNet-64, SCT achieves 1-step FID 2.42 and 2-step FID 1.55, a new SoTA for consistency models.

Consistency Model 학습 안정화 테크닉. 단일한 방법이라기보단 Phased Training 같은 여러 개선들의 결합이네요. (https://arxiv.org/abs/2405.18407) Consistency Model에 대한 안정성 개선 결과가 연달아 나오고 있군요.

<english>
Training stability techniques of consistency models. It is a kind of combination of improvements like phased training. (https://arxiv.org/abs/2405.18407) Many results on training stabilities of consistency models appears recently.
</english>

#diffusion

# Links

[[240528 Phased Consistency Model.md]]