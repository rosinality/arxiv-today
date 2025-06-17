https://arxiv.org/abs/2408.11049

*MagicDec: Breaking the Latency-Throughput Tradeoff for Long Context Generation with Speculative Decoding* (Jian Chen, Vashisth Tiwari, Ranajoy Sadhukhan, Zhuoming Chen, Jinyuan Shi, Ian En-Hsu Yen, Beidi Chen)

> Large Language Models (LLMs) have become more prevalent in long-context applications such as interactive chatbots, document analysis, and agent workflows, but it is challenging to serve long-context requests with low latency and high throughput. Speculative decoding (SD) is a widely used technique to reduce latency without sacrificing performance but the conventional wisdom suggests that its efficacy is limited to small batch sizes. In MagicDec, we show that surprisingly SD can achieve speedup even for a high throughput inference regime for moderate to long sequences. More interestingly, an intelligent drafting strategy can achieve better speedup with increasing batch size based on our rigorous analysis. MagicDec first identifies the bottleneck shifts with increasing batch size and sequence length, and uses these insights to deploy speculative decoding more effectively for high throughput inference. Then, it leverages draft models with sparse KV cache to address the KV bottleneck that scales with both sequence length and batch size.

시퀀스 길이가 길다면 배치 크기가 큰 경우에도 효과적인 Speculative Decoding. 배치 크기가 커지면 Memory bound였던 문제가 Compute bound로 이동하는데, 여기서 다시 시퀀스 길이가 길어지면 Memory bound로 이동한다고 하네요.

이 특성을 활용하자면 Drafter가 시퀀스 크기의 증가에 따른 메모리 사용량 증가가 없어야 하죠.

#efficiency 