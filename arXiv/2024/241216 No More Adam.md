https://arxiv.org/abs/2412.11768

*No More Adam: Learning Rate Scaling at Initialization is All You Need* (Minghao Xu, Lichuan Xiang, Xu Cai, Hongkai Wen)

> In this work, we question the necessity of adaptive gradient methods for training deep neural networks. SGD-SaI is a simple yet effective enhancement to stochastic gradient descent with momentum (SGDM). SGD-SaI performs learning rate Scaling at Initialization (SaI) to distinct parameter groups, guided by their respective gradient signal-to-noise ratios (g-SNR). By adjusting learning rates without relying on adaptive second-order momentum, SGD-SaI helps prevent training imbalances from the very first iteration and cuts the optimizer's memory usage by half compared to AdamW. Despite its simplicity and efficiency, SGD-SaI consistently matches or outperforms AdamW in training a variety of Transformer-based tasks, effectively overcoming a long-standing challenge of using SGD for training Transformers. SGD-SaI excels in ImageNet-1K classification with Vision Transformers(ViT) and GPT-2 pretraining for large language models (LLMs, transformer decoder-only), demonstrating robustness to hyperparameter variations and practicality for diverse applications. We further tested its robustness on tasks like LoRA fine-tuning for LLMs and diffusion models, where it consistently outperforms state-of-the-art optimizers. From a memory efficiency perspective, SGD-SaI achieves substantial memory savings for optimizer states, reducing memory usage by 5.93 GB for GPT-2 (1.5B parameters) and 25.15 GB for Llama2-7B compared to AdamW in full-precision training settings.

Second order Momentum 대신 그래디언트의 SNR로 LR Adaptation을 하는데, 그래디언트의 SNR은 학습 첫 Iteration과 그다지 달라지지 않으니 첫 Iteration에서 계산하고 계속 사용할 수 있다는 아이디어. 수렴 속도는 느리지만 학습 마지막에는 결국 AdamW와 비슷하다는 이야기를 하는군요.

<english>
Adapting LR using gradient SNR instead of second order momentum, and as gradient SNR is changes not much from the first iteration of training, reuses it after computing at the first iteration. The author says convergence rate is slower but at the end of training results is similar to AdamW.
</english>

#optimizer 