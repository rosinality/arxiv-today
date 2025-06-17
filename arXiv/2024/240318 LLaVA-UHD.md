https://arxiv.org/abs/2403.11703

*LLaVA-UHD: an LMM Perceiving Any Aspect Ratio and High-Resolution Images* (Ruyi Xu, Yuan Yao, Zonghao Guo, Junbo Cui, Zanlin Ni, Chunjiang Ge, Tat-Seng Chua, Zhiyuan Liu, Maosong Sun, Gao Huang)

> Visual encoding constitutes the basis of large multimodal models (LMMs) in understanding the visual world. Conventional LMMs process images in fixed sizes and limited resolutions, while recent explorations in this direction are limited in adaptivity, efficiency, and even correctness. In this work, we first take GPT-4V and LLaVA-1.5 as representative examples and expose systematic flaws rooted in their visual encoding strategy. To address the challenges, we present LLaVA-UHD, a large multimodal model that can efficiently perceive images in any aspect ratio and high resolution. LLaVA-UHD includes three key components: (1) An image modularization strategy that divides native-resolution images into smaller variable-sized slices for efficient and extensible encoding, (2) a compression module that further condenses image tokens from visual encoders, and (3) a spatial schema to organize slice tokens for LLMs. Comprehensive experiments show that LLaVA-UHD outperforms established LMMs trained with 2-3 orders of magnitude more data on 9 benchmarks. Notably, our model built on LLaVA-1.5 336x336 supports 6 times larger (i.e., 672x1088) resolution images using only 94% inference computation, and achieves 6.4 accuracy improvement on TextVQA. Moreover, the model can be efficiently trained in academic settings, within 23 hours on 8 A100 GPUs (vs. 26 hours of LLaVA-1.5). We make the data and code publicly available at https://github.com/thunlp/LLaVA-UHD.

GPT-4V의 Overlapping Window를 사용한 이미지 크롭과 LLaVA-1.5의 패딩 사용에서 발생하는 문제에서 시작하는군요. 패딩과 Overlap 없이 이미지를 잘 자르는 전략을 제안하고 있습니다. ViT 자체를 Multiple Aspect Ratio에 대해 학습시켜놓는 것이 유용할 것 같다는 느낌이 있네요. (https://arxiv.org/abs/2307.06304)

#vision-language

# Links

[[230712 Patch n' Pack.md]]