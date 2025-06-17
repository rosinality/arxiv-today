https://arxiv.org/abs/2411.07975

*JanusFlow: Harmonizing Autoregression and Rectified Flow for Unified Multimodal Understanding and Generation* (Yiyang Ma, Xingchao Liu, Xiaokang Chen, Wen Liu, Chengyue Wu, Zhiyu Wu, Zizheng Pan, Zhenda Xie, Haowei Zhang, Xingkai yu, Liang Zhao, Yisong Wang, Jiaying Liu, Chong Ruan)

> We present JanusFlow, a powerful framework that unifies image understanding and generation in a single model. JanusFlow introduces a minimalist architecture that integrates autoregressive language models with rectified flow, a state-of-the-art method in generative modeling. Our key finding demonstrates that rectified flow can be straightforwardly trained within the large language model framework, eliminating the need for complex architectural modifications. To further improve the performance of our unified model, we adopt two key strategies: (i) decoupling the understanding and generation encoders, and (ii) aligning their representations during unified training. Extensive experiments show that JanusFlow achieves comparable or superior performance to specialized models in their respective domains, while significantly outperforming existing unified approaches across standard benchmarks. This work represents a step toward more efficient and versatile vision-language models.

DeepSeek은 이미지 인식과 생성을 분리하는 시도를 좀 더 한 모양이네요. (https://arxiv.org/abs/2410.13848) 인식과 생성을 분리한다면 사실 생성을 Autoregressive 모델로 할 필요가 없으니 Rectified Flow를 생성에 사용했습니다.

<english>
DeepSeek did more trial on separating image recognition and generation. (https://arxiv.org/abs/2410.13848) If we want to separate recognition and generation actually we don't need to do generation in autoregressive manner. So they tried to use rectified flow.
</english>

#image-generation #multimodal #flow-matching

# Links

[[241017 Janus.md]]