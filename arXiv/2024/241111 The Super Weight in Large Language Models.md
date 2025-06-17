https://arxiv.org/abs/2411.07191

*The Super Weight in Large Language Models* (Mengxia Yu, De Wang, Qi Shan, Colorado Reed, Alvin Wan)

> Recent works have shown a surprising result: a small fraction of Large Language Model (LLM) parameter outliers are disproportionately important to the quality of the model. LLMs contain billions of parameters, so these small fractions, such as 0.01%, translate to hundreds of thousands of parameters. In this work, we present an even more surprising finding: Pruning as few as a single parameter can destroy an LLM's ability to generate text -- increasing perplexity by 3 orders of magnitude and reducing zero-shot accuracy to guessing. We propose a data-free method for identifying such parameters, termed super weights, using a single forward pass through the model. We additionally find that these super weights induce correspondingly rare and large activation outliers, termed super activations. When preserved with high precision, super activations can improve simple round-to-nearest quantization to become competitive with state-of-the-art methods. For weight quantization, we similarly find that by preserving the super weight and clipping other weight outliers, round-to-nearest quantization can scale to much larger block sizes than previously considered. To facilitate further research into super weights, we provide an index of super weight coordinates for common, openly available LLMs.

트랜스포머 LLM에는 극소수지만 성능에 절대적인 영향을 미치는 가중치가 있다는 분석. 생각보다 초기 레이어에 있고 이를 억제하면 Stopword만 생성하게 되는군요.

Super Weight의 효과가 아웃라이어로 모두 설명되는 것은 아니겠지만 아웃라이어와 관련해선 요즘 Adam과 회전을 통한 분석이 재미있네요. (https://arxiv.org/abs/2405.19279, https://arxiv.org/abs/2409.11321, https://arxiv.org/abs/2410.19964, https://arxiv.org/abs/2410.17174)

<english>
Analysis that in transformer LLMs there are weights which is very few but has sheer importance on model performances. It locates earlier layers than I thought and suppress it causing model to generate only stopwords.

Effect of super weight is cannot be all explained by outliers, but I think recent studies on outliers that links it with Adam and rotation. (https://arxiv.org/abs/2405.19279, https://arxiv.org/abs/2409.11321, https://arxiv.org/abs/2410.19964, https://arxiv.org/abs/2410.17174)
</english>

#quantization #transformer

# Links

[[240917 SOAP.md]]