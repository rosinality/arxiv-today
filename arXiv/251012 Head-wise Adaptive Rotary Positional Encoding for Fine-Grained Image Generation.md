https://arxiv.org/abs/2510.10489

*Head-wise Adaptive Rotary Positional Encoding for Fine-Grained Image Generation* (Jiaye Li, Baoyou Chen, Hui Li, Zilong Dong, Jingdong Wang, Siyu Zhu)

> Transformers rely on explicit positional encoding to model structure in data. While Rotary Position Embedding (RoPE) excels in 1D domains, its application to image generation reveals significant limitations such as fine-grained spatial relation modeling, color cues, and object counting. This paper identifies key limitations of standard multi-dimensional RoPE-rigid frequency allocation, axis-wise independence, and uniform head treatment-in capturing the complex structural biases required for fine-grained image generation. We propose HARoPE, a head-wise adaptive extension that inserts a learnable linear transformation parameterized via singular value decomposition (SVD) before the rotary mapping. This lightweight modification enables dynamic frequency reallocation, semantic alignment of rotary planes, and head-specific positional receptive fields while rigorously preserving RoPE's relative-position property. Extensive experiments on class-conditional ImageNet and text-to-image generation (Flux and MMDiT) demonstrate that HARoPE consistently improves performance over strong RoPE baselines and other extensions. The method serves as an effective drop-in replacement, offering a principled and adaptable solution for enhancing positional awareness in transformer-based image generative models.

더 나은 공간 모델링을 위해 RoPE 전에 헤드별 Linear Projection을 추가.

<english>
Adding head-specific linear projection before RoPE for better spatial relation modeling.
</english>

#positional-encoding #diffusion #image-generation 