https://arxiv.org/abs/2407.10969

*Q-Sparse: All Large Language Models can be Fully Sparsely-Activated* (Hongyu Wang, Shuming Ma, Ruiping Wang, Furu Wei)

> We introduce, Q-Sparse, a simple yet effective approach to training sparsely-activated large language models (LLMs). Q-Sparse enables full sparsity of activations in LLMs which can bring significant efficiency gains in inference. This is achieved by applying top-K sparsification to the activations and the straight-through-estimator to the training. The key results from this work are, (1) Q-Sparse can achieve results comparable to those of baseline LLMs while being much more efficient at inference time; (2) We present an inference-optimal scaling law for sparsely-activated LLMs; (3) Q-Sparse is effective in different settings, including training-from-scratch, continue-training of off-the-shelf LLMs, and finetuning; (4) Q-Sparse works for both full-precision and 1-bit LLMs (e.g., BitNet b1.58). Particularly, the synergy of BitNet b1.58 and Q-Sparse (can be equipped with MoE) provides the cornerstone and a clear path to revolutionize the efficiency, including cost and energy consumption, of future LLMs.

Top-K로 Activation을 Sparse하게 만드는 방법 + Quantization. Bitnet b1.58도 아직 잘 검증되지 않은 상태에서 추가적인 Activation Sparsity가 올라간 결과가 나온 형태라 좀 묘하긴 하네요.

#quantization #sparsity 