https://arxiv.org/abs/2503.09573

*Block Diffusion: Interpolating Between Autoregressive and Diffusion Language Models* (Marianne Arriola, Aaron Gokaslan, Justin T Chiu, Zhihan Yang, Zhixuan Qi, Jiaqi Han, Subham Sekhar Sahoo, Volodymyr Kuleshov)

> Diffusion language models offer unique benefits over autoregressive models due to their potential for parallelized generation and controllability, yet they lag in likelihood modeling and are limited to fixed-length generation. In this work, we introduce a class of block diffusion language models that interpolate between discrete denoising diffusion and autoregressive models. Block diffusion overcomes key limitations of both approaches by supporting flexible-length generation and improving inference efficiency with KV caching and parallel token sampling. We propose a recipe for building effective block diffusion models that includes an efficient training algorithm, estimators of gradient variance, and data-driven noise schedules to minimize the variance. Block diffusion sets a new state-of-the-art performance among diffusion models on language modeling benchmarks and enables generation of arbitrary-length sequences. We provide the code, along with the model weights and blog post on the project page: https://m-arriola.com/bd3lms/

Autoregression과 Diffusion이 부각되면 자연스럽게 블럭 단위의 Autoregression/Diffusion이 등장하기 마련이죠. Diffusion이 보통 관심을 갖는 이유은 Left-to-Right 순서의 제약을 해결해주지 못하게 되긴 합니다만.

<english>
When autoregression and diffusion got a spotlight, naturally block level autoregression/diffusion would appear. But it cannot resolve the problem of left-to-right ordering which is the reason why diffusion gain a traction.
</english>

#autoregressive-model #diffusion 