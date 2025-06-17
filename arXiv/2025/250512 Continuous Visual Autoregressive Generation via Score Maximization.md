https://arxiv.org/abs/2505.07812

*Continuous Visual Autoregressive Generation via Score Maximization* (Chenze Shao, Fandong Meng, Jie Zhou)

> Conventional wisdom suggests that autoregressive models are used to process discrete data. When applied to continuous modalities such as visual data, Visual AutoRegressive modeling (VAR) typically resorts to quantization-based approaches to cast the data into a discrete space, which can introduce significant information loss. To tackle this issue, we introduce a Continuous VAR framework that enables direct visual autoregressive generation without vector quantization. The underlying theoretical foundation is strictly proper scoring rules, which provide powerful statistical tools capable of evaluating how well a generative model approximates the true distribution. Within this framework, all we need is to select a strictly proper score and set it as the training objective to optimize. We primarily explore a class of training objectives based on the energy score, which is likelihood-free and thus overcomes the difficulty of making probabilistic predictions in the continuous space. Previous efforts on continuous autoregressive generation, such as GIVT and diffusion loss, can also be derived from our framework using other strictly proper scores. Source code: https://github.com/shaochenze/EAR.

Quantization 대신 Energy Score를 사용해 Continuous한 입력에 대해 Visual Autoregression을 학습.

<english>
Training visual autoregression on continuous inputs by using energy score instead of quantization.
</english>

#autoregressive-model #image-generation 