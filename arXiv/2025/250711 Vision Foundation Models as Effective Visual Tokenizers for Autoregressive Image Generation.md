https://arxiv.org/abs/2507.08441

*Vision Foundation Models as Effective Visual Tokenizers for Autoregressive Image Generation* (Anlin Zheng, Xin Wen, Xuanyang Zhang, Chuofan Ma, Tiancai Wang, Gang Yu, Xiangyu Zhang, Xiaojuan Qi)

> Leveraging the powerful representations of pre-trained vision foundation models -- traditionally used for visual comprehension -- we explore a novel direction: building an image tokenizer directly atop such models, a largely underexplored area. Specifically, we employ a frozen vision foundation model as the encoder of our tokenizer. To enhance its effectiveness, we introduce two key components: (1) a region-adaptive quantization framework that reduces redundancy in the pre-trained features on regular 2D grids, and (2) a semantic reconstruction objective that aligns the tokenizer's outputs with the foundation model's representations to preserve semantic fidelity. Based on these designs, our proposed image tokenizer, VFMTok, achieves substantial improvements in image reconstruction and generation quality, while also enhancing token efficiency. It further boosts autoregressive (AR) generation -- achieving a gFID of 2.07 on ImageNet benchmarks, while accelerating model convergence by three times, and enabling high-fidelity class-conditional synthesis without the need for classifier-free guidance (CFG). The code will be released publicly to benefit the community.

프리트레이닝된 이미지 인코더와 Deformable Attention을 사용한 이미지 토크나이저.

#vq 