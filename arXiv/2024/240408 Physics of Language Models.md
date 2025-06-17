https://arxiv.org/abs/2404.05405

*Physics of Language Models: Part 3.3, Knowledge Capacity Scaling Laws* (Zeyuan Allen-Zhu, Yuanzhi Li)

> Scaling laws describe the relationship between the size of language models and their capabilities. Unlike prior studies that evaluate a model's capability via loss or benchmarks, we estimate the number of knowledge bits a model stores. We focus on factual knowledge represented as tuples, such as (USA, capital, Washington D.C.) from a Wikipedia page. Through multiple controlled datasets, we establish that language models can and only can store 2 bits of knowledge per parameter, even when quantized to int8, and such knowledge can be flexibly extracted for downstream applications. Consequently, a 7B model can store 14B bits of knowledge, surpassing the English Wikipedia and textbooks combined based on our estimation. More broadly, we present 12 results on how (1) training duration, (2) model architecture, (3) quantization, (4) sparsity constraints such as MoE, and (5) data signal-to-noise ratio affect a model's knowledge storage capacity. Notable insights include: * The GPT-2 architecture, with rotary embedding, matches or even surpasses LLaMA/Mistral architectures in knowledge storage, particularly over shorter training durations. This arises because LLaMA/Mistral uses GatedMLP, which is less stable and harder to train. * Prepending training data with domain names (e.g., wikipedia.org) significantly increases a model's knowledge capacity. Language models can autonomously identify and prioritize domains rich in knowledge, optimizing their storage capacity.

LLM에 지식이 얼마나 저장되는가에 대한 Scaling Law. 가공의 신상명세 데이터를 사용해서 신상명세의 항목에 대한 Cross Entropy를 측정합니다.

다양한 모델 세팅에서 하나의 파라미터당 2 bit가 들어간다는 것을 발견했습니다. MoE를 사용해서 총 파라미터가 증가하는 경우에도 이 값이 아주 크게 감소하지 않는다는 것, 8 bit Quantization 까지는 문제가 없다는 것, (여기서는 불필요한 신상명세를 증가시키는 것으로 모사한) 저퀄리티의 데이터 추가가 이 값을 크게 떨어뜨린다는 것을 발견했습니다.

#scaling-law 