https://arxiv.org/abs/2404.08801

*Megalodon: Efficient LLM Pretraining and Inference with Unlimited Context Length* (Xuezhe Ma, Xiaomeng Yang, Wenhan Xiong, Beidi Chen, Lili Yu, Hao Zhang, Jonathan May, Luke Zettlemoyer, Omer Levy, Chunting Zhou)

> The quadratic complexity and weak length extrapolation of Transformers limits their ability to scale to long sequences, and while sub-quadratic solutions like linear attention and state space models exist, they empirically underperform Transformers in pretraining efficiency and downstream task accuracy. We introduce Megalodon, a neural architecture for efficient sequence modeling with unlimited context length. Megalodon inherits the architecture of Mega (exponential moving average with gated attention), and further introduces multiple technical components to improve its capability and stability, including complex exponential moving average (CEMA), timestep normalization layer, normalized attention mechanism and pre-norm with two-hop residual configuration. In a controlled head-to-head comparison with Llama2, Megalodon achieves better efficiency than Transformer in the scale of 7 billion parameters and 2 trillion training tokens. Megalodon reaches a training loss of 1.70, landing mid-way between Llama2-7B (1.75) and 13B (1.67). Code: https://github.com/XuezheMax/megalodon

이전에 나왔던 Mega (https://arxiv.org/abs/2209.10655) 모델의 개선이군요. EMA 기반 모델인데 기본적으로 State Space Model과 비슷합니다. Chunkwise Attention이 들어간다는 점에서는 이미 하이브리드 모델이라고 할 수도 있겠군요.

Mega에 복소수 기반 EMA, Causal Group Norm, FFN에 레이어를 건너뛴 Skip Connection을 연결하는 등의 트릭을 사용했군요. 7B/2T 레벨의 학습을 진행했습니다. 사실 Chunkwise Attention이 그렇게 미덥지(?) 않긴 합니다만.

#state-space-model

# Links

[[220921 Mega.md]]