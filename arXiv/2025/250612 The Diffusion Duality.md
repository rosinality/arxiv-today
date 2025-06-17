https://arxiv.org/abs/2506.10892

*The Diffusion Duality* (Subham Sekhar Sahoo, Justin Deschenaux, Aaron Gokaslan, Guanghan Wang, Justin Chiu, Volodymyr Kuleshov)

> Uniform-state discrete diffusion models hold the promise of fast text generation due to their inherent ability to self-correct. However, they are typically outperformed by autoregressive models and masked diffusion models. In this work, we narrow this performance gap by leveraging a key insight: Uniform-state diffusion processes naturally emerge from an underlying Gaussian diffusion. Our method, Duo, transfers powerful techniques from Gaussian diffusion to improve both training and sampling. First, we introduce a curriculum learning strategy guided by the Gaussian process, doubling training speed by reducing variance. Models trained with curriculum learning surpass autoregressive models in zero-shot perplexity on 3 of 7 benchmarks. Second, we present Discrete Consistency Distillation, which adapts consistency distillation from the continuous to the discrete setting. This algorithm unlocks few-step generation in diffusion language models by accelerating sampling by two orders of magnitude. We provide the code and model checkpoints on the project page: http://s-sahoo.github.io/duo

Gaussian Diffusion을 Uniform Discrete Diffusion과 argmax로 연결한 다음 Gaussian Diffusion의 테크닉을 Discrete Diffusion에 적용했군요.

<english>
Connecting gaussian diffusion with uniform discrete diffusion using argmax, then applied techniques from gaussian diffusion to discrete diffusion.
</english>

#lm #diffusion 