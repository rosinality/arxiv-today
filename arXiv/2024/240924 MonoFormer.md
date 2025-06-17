https://arxiv.org/abs/2409.16280

*MonoFormer: One Transformer for Both Diffusion and Autoregression* (Chuyang Zhao, Yuxing Song, Wenhao Wang, Haocheng Feng, Errui Ding, Yifan Sun, Xinyan Xiao, Jingdong Wang)

> Most existing multimodality methods use separate backbones for autoregression-based discrete text generation and diffusion-based continuous visual generation, or the same backbone by discretizing the visual data to use autoregression for both text and visual generation. In this paper, we propose to study a simple idea: share one transformer for both autoregression and diffusion. The feasibility comes from two main aspects: (i) Transformer is successfully applied to diffusion for visual generation, and (ii) transformer training for autoregression and diffusion is very similar, and the difference merely lies in that diffusion uses bidirectional attention mask and autoregression uses causal attention mask. Experimental results show that our approach achieves comparable image generation performance to current state-of-the-art methods as well as maintains the text generation capability. The project is publicly available at https://monoformer.github.io/.

Transfusion과 (https://www.arxiv.org/abs/2408.11039) 비슷한 Autoregresssive 텍스트 생성과 Diffusion 기반 이미지 생성.

#diffusion #autoregressive-model #text-to-image

# Links

[[240820 Transfusion.md]]