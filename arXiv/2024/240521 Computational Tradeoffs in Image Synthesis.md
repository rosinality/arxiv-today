https://arxiv.org/abs/2405.13218

*Computational Tradeoffs in Image Synthesis: Diffusion, Masked-Token, and Next-Token Prediction* (Maciej Kilian, Varun Japan, Luke Zettlemoyer)

> Nearly every recent image synthesis approach, including diffusion, masked-token prediction, and next-token prediction, uses a Transformer network architecture. Despite this common backbone, there has been no direct, compute controlled comparison of how these approaches affect performance and efficiency. We analyze the scalability of each approach through the lens of compute budget measured in FLOPs. We find that token prediction methods, led by next-token prediction, significantly outperform diffusion on prompt following. On image quality, while next-token prediction initially performs better, scaling trends suggest it is eventually matched by diffusion. We compare the inference compute efficiency of each approach and find that next token prediction is by far the most efficient. Based on our findings we recommend diffusion for applications targeting image quality and low latency; and next-token prediction when prompt following or throughput is more important.

Next Token Prediction vs Masked Token Prediction vs Diffusion의 Text-to-Image에 대한 Scaling Law. 흥미롭게도 Next Token Prediction이 가장 나은 성능을 찍고 있습니다. 다만 Scaling Curve의 경사가 Diffusion이 더 큰 것 같다는 느낌이 있네요.

추가로 LFQ (https://arxiv.org/abs/2310.05737) 의 사용도 흥미롭습니다.

#autoregressive-model #diffusion #scaling-law

# Links

[[231009 Language Model Beats Diffusion -- Tokenizer is Key to Visual Generation.md]]