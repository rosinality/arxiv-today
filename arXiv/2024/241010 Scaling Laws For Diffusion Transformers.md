https://arxiv.org/abs/2410.08184

*Scaling Laws For Diffusion Transformers* (Zhengyang Liang, Hao He, Ceyuan Yang, Bo Dai)

> Diffusion transformers (DiT) have already achieved appealing synthesis and scaling properties in content recreation, e.g., image and video generation. However, scaling laws of DiT are less explored, which usually offer precise predictions regarding optimal model size and data requirements given a specific compute budget. Therefore, experiments across a broad range of compute budgets, from 1e17 to 6e18 FLOPs are conducted to confirm the existence of scaling laws in DiT for the first time. Concretely, the loss of pretraining DiT also follows a power-law relationship with the involved compute. Based on the scaling law, we can not only determine the optimal model size and required data but also accurately predict the text-to-image generation loss given a model with 1B parameters and a compute budget of 1e21 FLOPs. Additionally, we also demonstrate that the trend of pre-training loss matches the generation performances (e.g., FID), even across various datasets, which complements the mapping from compute to synthesis quality and thus provides a predictable benchmark that assesses model performance and data quality at a reduced cost.

DiT에 대한 Scaling Law 추정. Autoregressive와 Diffusion의 Scaling Law의 지수 차이를 추정해보면 재미있지 않을까 싶습니다만 (https://arxiv.org/abs/2405.13218) 아직 모델 아키텍처가 발전하는 중이니 쉽지는 않겠네요.

<english>
Estimation of scaling law of DiT. It would be interesting to estimate difference of exponents between scaling law of autoregressive and diffusion models, (https://arxiv.org/abs/2405.13218) but as model architecture is continuously improving, it would be not easy.

#diffusion #scaling-law

# Links

[[240521 Computational Tradeoffs in Image Synthesis.md]]