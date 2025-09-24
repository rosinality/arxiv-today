https://arxiv.org/abs/2509.18824

*Hyper-Bagel: A Unified Acceleration Framework for Multimodal Understanding and Generation* (Yanzuo Lu, Xin Xia, Manlin Zhang, Huafeng Kuang, Jianbin Zheng, Yuxi Ren, Xuefeng Xiao)

> Unified multimodal models have recently attracted considerable attention for their remarkable abilities in jointly understanding and generating diverse content. However, as contexts integrate increasingly numerous interleaved multimodal tokens, the iterative processes of diffusion denoising and autoregressive decoding impose significant computational overhead. To address this, we propose Hyper-Bagel, a unified acceleration framework designed to simultaneously speed up both multimodal understanding and generation tasks. Our approach uses a divide-and-conquer strategy, employing speculative decoding for next-token prediction and a multi-stage distillation process for diffusion denoising. The framework delivers substantial performance gains, achieving over a 2x speedup in multimodal understanding. For generative tasks, our resulting lossless 6-NFE model yields a 16.67x speedup in text-to-image generation and a 22x speedup in image editing, all while preserving the high-quality output of the original model. We further develop a highly efficient 1-NFE model that enables near real-time interactive editing and generation. By combining advanced adversarial distillation with human feedback learning, this model achieves ultimate cost-effectiveness and responsiveness, making complex multimodal interactions seamless and instantaneous.

이미지 이해 및 생성 통합 모형을 Speculative Decoding과 (https://arxiv.org/abs/2503.01840) Diffusion Distillation으로 가속.

Accelerating unified image understanding and generation model through speculative decoding (https://arxiv.org/abs/2503.01840) and diffusion distillation.

#efficiency #image-generation #multimodal 