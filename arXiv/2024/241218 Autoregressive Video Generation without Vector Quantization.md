https://arxiv.org/abs/2412.14169

*Autoregressive Video Generation without Vector Quantization* (Haoge Deng, Ting Pan, Haiwen Diao, Zhengxiong Luo, Yufeng Cui, Huchuan Lu, Shiguang Shan, Yonggang Qi, Xinlong Wang)

> This paper presents a novel approach that enables autoregressive video generation with high efficiency. We propose to reformulate the video generation problem as a non-quantized autoregressive modeling of temporal frame-by-frame prediction and spatial set-by-set prediction. Unlike raster-scan prediction in prior autoregressive models or joint distribution modeling of fixed-length tokens in diffusion models, our approach maintains the causal property of GPT-style models for flexible in-context capabilities, while leveraging bidirectional modeling within individual frames for efficiency. With the proposed approach, we train a novel video autoregressive model without vector quantization, termed NOVA. Our results demonstrate that NOVA surpasses prior autoregressive video models in data efficiency, inference speed, visual fidelity, and video fluency, even with a much smaller model capacity, i.e., 0.6B parameters. NOVA also outperforms state-of-the-art image diffusion models in text-to-image generation tasks, with a significantly lower training cost. Additionally, NOVA generalizes well across extended video durations and enables diverse zero-shot applications in one unified model. Code and models are publicly available at https://github.com/baaivision/NOVA.

시간축으로는 프레임 단위 Autoregression, 각 프레임 내에서는 MAR (https://arxiv.org/abs/2406.11838). 프레임 내의 예측이 일종의 앵커를 사용하지 않고는 어려웠다고 하네요.

<english>
Frame level autoregression along time axis, and each frames predicted with MAR (https://arxiv.org/abs/2406.11838). The author says that predicting each frames was hard without some kind of anchor features.
</english>

#video-generation #diffusion #autoregressive-model

# Links

[[240617 Autoregressive Image Generation without Vector Quantization.md]]