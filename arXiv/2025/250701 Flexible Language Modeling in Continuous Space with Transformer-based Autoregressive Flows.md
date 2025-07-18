https://arxiv.org/abs/2507.00425

*Flexible Language Modeling in Continuous Space with Transformer-based Autoregressive Flows* (Ruixiang Zhang, Shuangfei Zhai, Jiatao Gu, Yizhe Zhang, Huangjie Zheng, Tianrong Chen, Miguel Angel Bautista, Josh Susskind, Navdeep Jaitly)

> Autoregressive models have driven remarkable progress in language modeling. Their foundational reliance on discrete tokens, unidirectional context, and single-pass decoding, while central to their success, also inspires the exploration of a design space that could offer new axes of modeling flexibility. In this work, we explore an alternative paradigm, shifting language modeling from a discrete token space to a continuous latent space. We propose a novel framework TarFlowLM, that employs transformer-based autoregressive normalizing flows to model these continuous representations. This approach unlocks substantial flexibility, enabling the construction of models that can capture global bi-directional context through stacked, alternating-direction autoregressive transformations, support block-wise generation with flexible token patch sizes, and facilitate a hierarchical multi-pass generation process. We further propose new mixture-based coupling transformations designed to capture complex dependencies within the latent space shaped by discrete data, and demonstrate theoretical connections to conventional discrete autoregressive models. Extensive experiments on language modeling benchmarks demonstrate strong likelihood performance and highlight the flexible modeling capabilities inherent in our framework.

Autoregressive Flow를 사용한 LM. 입출력은 VAE에 의존하네요. Diffusion도 그렇고 애플이 대안적 LM을 여럿 시도하는군요 (https://arxiv.org/abs/2506.20639).

<english>
A LM based on autoregressive flow. For inputs and outputs they used VAE. Like recent diffusion LMs, Apple tries various approaches for alternative LMs (https://arxiv.org/abs/2506.20639).
</english>

#flow #lm 