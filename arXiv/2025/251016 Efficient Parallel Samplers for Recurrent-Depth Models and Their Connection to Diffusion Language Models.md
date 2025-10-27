https://arxiv.org/abs/2510.14961

*Efficient Parallel Samplers for Recurrent-Depth Models and Their Connection to Diffusion Language Models* (Jonas Geiping, Xinyu Yang, Guinan Su)

> Language models with recurrent depth, also referred to as universal or looped when considering transformers, are defined by the capacity to increase their computation through the repetition of layers. Recent efforts in pretraining have demonstrated that these architectures can scale to modern language modeling tasks while exhibiting advantages in reasoning tasks. In this work, we examine the relationship between recurrent-depth models and diffusion language models. Building on their similarities, we develop a new diffusion forcing sampler for these models to accelerate generation. The sampler advances by decoding new tokens at every forward pass of the model, while the latent states of these tokens can be further refined in parallel through recurrence. Theoretically, generation with our sampler is strictly more expressive than the baseline autoregressive generation using the same time budget on modern hardware. Moreover, this sampler, based on principles from diffusion literature, can be directly applied to existing 3.5B recurrent-depth transformers without any tuning, leading to up to a 5x speedup. Consequently, our findings not only provide an efficient mechanism for parallelizing the extra computation in recurrent-depth models at inference, but also suggest that such models can be naturally viewed as strong continuous, though causal, diffusion language models.

Looped Autoregressive Transformer에 대한 Block Diffusion과 유사한 샘플링. Looped Transformer는 저자가 지적하는 것처럼 일종의 Latent Diffusion 모델일지도?

Block diffusion-like sampling for looped autoregressive transformers. Maybe looped transformers, as the authors suggest, are a kind of latent diffusion model?

#diffusion #transformer #autoregressive-model 