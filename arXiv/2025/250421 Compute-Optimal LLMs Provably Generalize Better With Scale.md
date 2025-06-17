https://arxiv.org/abs/2504.15208

*Compute-Optimal LLMs Provably Generalize Better With Scale* (Marc Finzi, Sanyam Kapoor, Diego Granziol, Anming Gu, Christopher De Sa, J. Zico Kolter, Andrew Gordon Wilson)

> Why do larger language models generalize better? To investigate this question, we develop generalization bounds on the pretraining objective of large language models (LLMs) in the compute-optimal regime, as described by the Chinchilla scaling laws. We introduce a novel, fully empirical Freedman-type martingale concentration inequality that tightens existing bounds by accounting for the variance of the loss function. This generalization bound can be decomposed into three interpretable components: the number of parameters per token, the loss variance, and the quantization error at a fixed bitrate. As compute-optimal language models are scaled up, the number of parameters per data point remains constant; however, both the loss variance and the quantization error decrease, implying that larger models should have smaller generalization gaps. We examine why larger models tend to be more quantizable from an information theoretic perspective, showing that the rate at which they can integrate new information grows more slowly than their capacity on the compute-optimal frontier. From these findings we produce a scaling law for the generalization gap, with bounds that become predictably stronger with scale.

Chinchilla Scaling을 할 때의 Generalization Bound에 대한 분석. Random Guess, Loss Variation, Smoothing, Quantization 항으로 구성되어 있는데 모델 크기 증가에 따라 Loss Variation과 Quantization 항은 감소한다고 하는군요.

<english>
Analysis on generalization bound when doing chinchilla scaling. It consist of random guess, loss variation, smoothing quantization terms, and the paper suggests loss variation and quantization reduces with increase of model sizes.
</english>

#llm #generalization 