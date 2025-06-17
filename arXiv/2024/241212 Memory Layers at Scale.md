https://arxiv.org/abs/2412.09764

*Memory Layers at Scale* (Vincent-Pierre Berges, Barlas Oğuz, Daniel Haziza, Wen-tau Yih, Luke Zettlemoyer, Gargi Gosh)

> Memory layers use a trainable key-value lookup mechanism to add extra parameters to a model without increasing FLOPs. Conceptually, sparsely activated memory layers complement compute-heavy dense feed-forward layers, providing dedicated capacity to store and retrieve information cheaply. This work takes memory layers beyond proof-of-concept, proving their utility at contemporary scale. On downstream tasks, language models augmented with our improved memory layer outperform dense models with more than twice the computation budget, as well as mixture-of-expert models when matched for both compute and parameters. We find gains are especially pronounced for factual tasks. We provide a fully parallelizable memory layer implementation, demonstrating scaling laws with up to 128B memory parameters, pretrained to 1 trillion tokens, comparing to base models with up to 8B parameters.

Sparse Key-Value Memory 계통 연구도 꽤 나오는군요. (https://arxiv.org/abs/2407.04153, https://arxiv.org/abs/2411.12364) 마찬가지로 Product Key Memory를 사용했네요. 지식을 따로 저장한다는 것은 흥미롭긴 하지만 VQ 쪽에서 보고되는 Sparse Update로 인한 문제를 생각하면 좀 까다로울 것 같습니다. (https://arxiv.org/abs/2411.02038, https://arxiv.org/abs/2412.02692)

<english>
Recently there are many studies related to sparse key-value memory. (https://arxiv.org/abs/2407.04153, https://arxiv.org/abs/2411.12364) This study also employed product key memory. It is interesting to store knowledges separately, but if we consider the problems originate from sparse update which frequently reported in VQ I think it would be quite picky (https://arxiv.org/abs/2411.02038, https://arxiv.org/abs/2412.02692).

#moe #sparsity

# Links

[[241104 Addressing Representation Collapse in Vector Quantized Models with One Linear Layer.md]]
[[241203 Taming Scalable Visual Tokenizer for Autoregressive Image Generation.md]]
[[241119 Ultra-Sparse Memory Network.md]]