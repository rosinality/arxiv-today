https://arxiv.org/abs/2501.16295

*Mixture-of-Mamba: Enhancing Multi-Modal State-Space Models with Modality-Aware Sparsity* (Weixin Liang, Junhong Shen, Genghan Zhang, Ning Dong, Luke Zettlemoyer, Lili Yu)

> State Space Models (SSMs) have emerged as efficient alternatives to Transformers for sequential modeling, but their inability to leverage modality-specific features limits their performance in multi-modal pretraining. Here, we propose Mixture-of-Mamba, a novel SSM architecture that introduces modality-aware sparsity through modality-specific parameterization of the Mamba block. Building on Mixture-of-Transformers (W. Liang et al. arXiv:2411.04996; 2024), we extend the benefits of modality-aware sparsity to SSMs while preserving their computational efficiency. We evaluate Mixture-of-Mamba across three multi-modal pretraining settings: Transfusion (interleaved text and continuous image tokens with diffusion loss), Chameleon (interleaved text and discrete image tokens), and an extended three-modality framework incorporating speech. Mixture-of-Mamba consistently reaches the same loss values at earlier training steps with significantly reduced computational costs. In the Transfusion setting, Mixture-of-Mamba achieves equivalent image loss using only 34.76% of the training FLOPs at the 1.4B scale. In the Chameleon setting, Mixture-of-Mamba reaches similar image loss with just 42.50% of the FLOPs at the 1.4B scale, and similar text loss with just 65.40% of the FLOPs. In the three-modality setting, MoM matches speech loss at 24.80% of the FLOPs at the 1.4B scale. Our ablation study highlights the synergistic effects of decoupling projection components, where joint decoupling yields greater gains than individual modifications. These results establish modality-aware sparsity as a versatile and effective design principle, extending its impact from Transformers to SSMs and setting new benchmarks in multi-modal pretraining. Our code can be accessed at https://github.com/Weixin-Liang/Mixture-of-Mamba

Mamba 기반 멀티모달 (Transfusion, https://arxiv.org/abs/2408.11039) 모델에서 모달리티별로 다른 Weight를 사용한다는 아이디어. 모달리티에 따라 Weight를 분리하는 것은 종종 나오는 아이디어인데 이쪽은 Mamba에 대해서 했군요.

Mamba-based multimodal models like Transfusion (https://arxiv.org/abs/2408.11039) are using modality-specific weights. It's a common idea to separate weights for different modalities, but this paper does it with Mamba.

#multimodal #diffusion #image-generation #state-space-model

# Links

[[240820 Transfusion.md]]