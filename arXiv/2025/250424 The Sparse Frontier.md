https://arxiv.org/abs/2504.17768

*The Sparse Frontier: Sparse Attention Trade-offs in Transformer LLMs* (Piotr Nawrot, Robert Li, Renjie Huang, Sebastian Ruder, Kelly Marchisio, Edoardo M. Ponti)

> Sparse attention offers a promising strategy to extend long-context capabilities in Transformer LLMs, yet its viability, its efficiency-accuracy trade-offs, and systematic scaling studies remain unexplored. To address this gap, we perform a careful comparison of training-free sparse attention methods at varying model scales, sequence lengths, and sparsity levels on a diverse collection of long-sequence tasks-including novel ones that rely on natural language while remaining controllable and easy to evaluate. Based on our experiments, we report a series of key findings: 1) an isoFLOPS analysis reveals that for very long sequences, larger and highly sparse models are preferable to smaller and dense ones. 2) The level of sparsity attainable while statistically guaranteeing accuracy preservation is higher during decoding than prefilling, and correlates with model size in the former. 3) There is no clear strategy that performs best across tasks and phases, with different units of sparsification or budget adaptivity needed for different scenarios. Even moderate sparsity levels often result in significant performance degradation on at least one task, highlighting that sparse attention is not a universal solution. 4) We introduce and validate novel scaling laws specifically tailored for sparse attention, providing evidence that our findings are likely to hold true beyond our range of experiments. Through these insights, we demonstrate that sparse attention is a key tool to enhance the capabilities of Transformer LLMs for processing longer sequences, but requires careful evaluation of trade-offs for performance-sensitive applications.

Sparse Attention에 대한 Scaling Law. 컨텍스트 길이가 길어지면 동일 FLOPS에서 우위가 발생하는군요. 학습 없이 Sparse Attention으로 전환한 결과이니 프리트레이닝 시점에서부터 Sparse Attention을 채택한 경우 특성이 좀 더 나아지겠죠.

<english>
Scaling law for sparse attention. As context length became larger it shows advantage on similar FLOPS. As this result based on adopt sparse attention without training, we can expect better characteristics if we adopt it from the pretraining.
</english>

#sparsity #attention #scaling-law 