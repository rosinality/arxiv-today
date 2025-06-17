https://arxiv.org/abs/2402.08644

*Tandem Transformers for Inference Efficient LLMs* (Aishwarya P S, Pranav Ajit Nair, Yashas Samaga, Toby Boyd, Sanjiv Kumar, Prateek Jain, Praneeth Netrapalli)

> The autoregressive nature of conventional large language models (LLMs) inherently limits inference speed, as tokens are generated sequentially. While speculative and parallel decoding techniques attempt to mitigate this, they face limitations: either relying on less accurate smaller models for generation or failing to fully leverage the base LLM's representations. We introduce a novel architecture, Tandem transformers, to address these issues. This architecture uniquely combines (1) a small autoregressive model and (2) a large model operating in block mode (processing multiple tokens simultaneously). The small model's predictive accuracy is substantially enhanced by granting it attention to the large model's richer representations. On the PaLM2 pretraining dataset, a tandem of PaLM2-Bison and PaLM2-Gecko demonstrates a 3.3% improvement in next-token prediction accuracy over a standalone PaLM2-Gecko, offering a 1.16x speedup compared to a PaLM2-Otter model with comparable downstream performance. We further incorporate the tandem model within the speculative decoding (SPEED) framework where the large model validates tokens from the small model. This ensures that the Tandem of PaLM2-Bison and PaLM2-Gecko achieves substantial speedup (around 1.14x faster than using vanilla PaLM2-Gecko in SPEED) while maintaining identical downstream task accuracy.

구글의 새로운 모델 병합 시도군요. 작은 LM이 큰 LM의 임베딩을 참조할 수 있도록 연결합니다. 추론 시점에서 작은 모델로 디코딩한 다음 디코딩 결과를 큰 모델에 주입해서 검증하는 Speculative Decoding을 할 수 있습니다.

그나저나 구글은 Speculative Decoding을 SPEED라고 부르나 보네요.

#efficiency 