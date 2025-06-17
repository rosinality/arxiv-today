https://arxiv.org/abs/2506.01928

*Esoteric Language Models* (Subham Sekhar Sahoo, Zhihan Yang, Yash Akhauri, Johnna Liu, Deepansha Singh, Zhoujun Cheng, Zhengzhong Liu, Eric Xing, John Thickstun, Arash Vahdat)

> Diffusion-based language models offer a compelling alternative to autoregressive (AR) models by enabling parallel and controllable generation. Among this family of models, Masked Diffusion Models (MDMs) achieve the strongest performance but still underperform AR models in perplexity and lack key inference-time efficiency features--most notably, KV caching. In this work, we introduce Eso-LMs, a new family of models that fuses AR and MDM paradigms, enabling smooth interpolation between their perplexities while overcoming their respective limitations. Eso-LMs set a new state of the art on standard language modeling benchmarks. Crucially, we are the **first to introduce KV caching for MDMs** while preserving parallel generation, significantly improving inference efficiency. Combined with an optimized sampling schedule, our method achieves up to **65x** faster inference than standard MDMs and **4x** faster inference than prior semi-autoregressive approaches. We provide the code and model checkpoints on the project page: [http://s-sahoo.github.io/Eso-LMs](http://s-sahoo.github.io/Eso-LMs)

Diffusion과 Autoregressive 모델을 내삽하는 모델. KV 캐시를 허용하고 디노이징할 토큰만 Forward하는 구조로 속도를 더 높였군요.

<english>
A model interploates diffusion and autoregressive model. Sampling speed enhance with design that allows KV cache and forwards tokens that would be denoised.
</english>

#diffusion #autoregressive-model 