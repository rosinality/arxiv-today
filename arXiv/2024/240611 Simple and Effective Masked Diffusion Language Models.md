https://arxiv.org/abs/2406.07524

*Simple and Effective Masked Diffusion Language Models* (Subham Sekhar Sahoo, Marianne Arriola, Yair Schiff, Aaron Gokaslan, Edgar Marroquin, Justin T Chiu, Alexander Rush, Volodymyr Kuleshov)

> While diffusion models excel at generating high-quality images, prior work reports a significant performance gap between diffusion and autoregressive (AR) methods in language modeling. In this work, we show that simple masked discrete diffusion is more performant than previously thought. We apply an effective training recipe that improves the performance of masked diffusion models and derive a simplified, Rao-Blackwellized objective that results in additional improvements. Our objective has a simple form -- it is a mixture of classical masked language modeling losses -- and can be used to train encoder-only language models that admit efficient samplers, including ones that can generate arbitrary lengths of text semi-autoregressively like a traditional language model. On language modeling benchmarks, a range of masked diffusion models trained with modern engineering practices achieves a new state-of-the-art among diffusion models, and approaches AR perplexity. We release our code at: https://github.com/kuleshov-group/mdlm

Masked Diffusion을 사용한 텍스트 생성. 기존의 Masked Diffusion보다 더 심플하고 분산이 작은 Objective를 사용했다는 것이 핵심 같네요.

Diffusion을 사용한 텍스트 생성이 토큰의 생성 순서 문제를 잡을 수 있지 않을까 하는 생각을 합니다. 다만 요즘 스트리밍 생성에 관심이 집중되고 있는 터라 예전보단 약간 우려가 되긴 하네요.

#diffusion 