https://arxiv.org/abs/2502.05795

*The Curse of Depth in Large Language Models* (Wenfang Sun, Xinyuan Song, Pengxiang Li, Lu Yin, Yefeng Zheng, Shiwei Liu)

> In this paper, we introduce the Curse of Depth, a concept that highlights, explains, and addresses the recent observation in modern Large Language Models(LLMs) where nearly half of the layers are less effective than expected. We first confirm the wide existence of this phenomenon across the most popular families of LLMs such as Llama, Mistral, DeepSeek, and Qwen. Our analysis, theoretically and empirically, identifies that the underlying reason for the ineffectiveness of deep layers in LLMs is the widespread usage of Pre-Layer Normalization (Pre-LN). While Pre-LN stabilizes the training of Transformer LLMs, its output variance exponentially grows with the model depth, which undesirably causes the derivative of the deep Transformer blocks to be an identity matrix, and therefore barely contributes to the training. To resolve this training pitfall, we propose LayerNorm Scaling, which scales the variance of output of the layer normalization inversely by the square root of its depth. This simple modification mitigates the output variance explosion of deeper Transformer layers, improving their contribution. Our experimental results, spanning model sizes from 130M to 1B, demonstrate that LayerNorm Scaling significantly enhances LLM pre-training performance compared to Pre-LN. Moreover, this improvement seamlessly carries over to supervised fine-tuning. All these gains can be attributed to the fact that LayerNorm Scaling enables deeper layers to contribute more effectively during training.

Pre LN에서 레이어의 기여도가 낮아지는 문제에 대한 답. 레이어 번호로 크기를 조정하는 것은 종종 시도되는 방법이었는데 여기서는 블록의 출력 레이어가 아니라 Pre LN의 출력을 축소시켰군요.

MiniMax-01에서는 아예 DeepNorm을 썼죠. (https://arxiv.org/abs/2501.08313, https://arxiv.org/abs/2203.00555) 늘 재미있는 주제이긴 합니다.

<english>
Solution for the problem of Pre LN reducing the contribution of each layers. Scaling with layer index is tried previously, but in the paper instead of the output layer in blocks they scaled output of Pre LN.

MiniMax-01 tried DeepNorm for this problem. (https://arxiv.org/abs/2501.08313, https://arxiv.org/abs/2203.00555) It's always interesting problem.
</english>

#normalization #transformer

# Links

[[220301 DeepNet.md]]
[[250114 MiniMax-01.md]]