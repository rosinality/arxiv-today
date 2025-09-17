https://arxiv.org/abs/2507.13575

*Apple Intelligence Foundation Language Models: Tech Report 2025* (Apple)

> We introduce two multilingual, multimodal foundation language models that power Apple Intelligence features across Apple devices and services: i a 3B-parameter on-device model optimized for Apple silicon through architectural innovations such as KV-cache sharing and 2-bit quantization-aware training; and ii a scalable server model built on a novel Parallel-Track Mixture-of-Experts PT-MoE transformer that combines track parallelism, mixture-of-experts sparse computation, and interleaved global-local attention to deliver high quality with competitive cost on Apple's Private Cloud Compute platform. Both models are trained on large-scale multilingual and multimodal datasets sourced via responsible web crawling, licensed corpora, and high-quality synthetic data, then further refined with supervised fine-tuning and reinforcement learning on a new asynchronous platform. The resulting models support several additional languages while understanding images and executing tool calls. In public benchmarks and human evaluations, both the server model and the on-device model match or surpass comparably sized open baselines. A new Swift-centric Foundation Models framework exposes guided generation, constrained tool calling, and LoRA adapter fine-tuning, allowing developers to integrate these capabilities with a few lines of code. The latest advancements in Apple Intelligence models are grounded in our Responsible AI approach with safeguards like content filtering and locale-specific evaluation, as well as our commitment to protecting our users' privacy with innovations like Private Cloud Compute.

애플 파운데이션 모델. 흥미롭게도 새로운 구조를 사용했군요. 모델을 트랙이라는 블럭으로 나누고 병렬적으로 실행한 다음 합치는 형태네요.

<english>
Apple Foundation Model. Interestingly they used novel architecture. Splits models into blocks called track, run it parallel and synchronizes it.
</english>

#transformer #llm 