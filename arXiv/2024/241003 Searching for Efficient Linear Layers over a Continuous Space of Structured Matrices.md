https://arxiv.org/abs/2410.02117

*Searching for Efficient Linear Layers over a Continuous Space of Structured Matrices* (Andres Potapczynski, Shikai Qiu, Marc Finzi, Christopher Ferri, Zixi Chen, Micah Goldblum, Bayan Bruss, Christopher De Sa, Andrew Gordon Wilson)

> Dense linear layers are the dominant computational bottleneck in large neural networks, presenting a critical need for more efficient alternatives. Previous efforts focused on a small number of hand-crafted structured matrices and neglected to investigate whether these structures can surpass dense layers in terms of compute-optimal scaling laws when both the model size and training examples are optimally allocated. In this work, we present a unifying framework that enables searching among all linear operators expressible via an Einstein summation. This framework encompasses many previously proposed structures, such as low-rank, Kronecker, Tensor-Train, Block Tensor-Train (BTT), and Monarch, along with many novel structures. To analyze the framework, we develop a taxonomy of all such operators based on their computational and algebraic properties and show that differences in the compute-optimal scaling laws are mostly governed by a small number of variables that we introduce. Namely, a small $\omega$ (which measures parameter sharing) and large $\psi$ (which measures the rank) reliably led to better scaling laws. Guided by the insight that full-rank structures that maximize parameters per unit of compute perform the best, we propose BTT-MoE, a novel Mixture-of-Experts (MoE) architecture obtained by sparsifying computation in the BTT structure. In contrast to the standard sparse MoE for each entire feed-forward network, BTT-MoE learns an MoE in every single linear layer of the model, including the projection matrices in the attention blocks. We find BTT-MoE provides a substantial compute-efficiency gain over dense layers and standard MoE.

Tensor Train 같은 Structured Matrix를 사용하는 방법들을 einsum으로 통합한 다음 Scaling Law를 추정. 결과적으로는 Dense 세팅을 능가하는 경우는 없었습니다. MoE의 경우에는 Block Tensor Train이 조금 더 나은 결과가 나타났는데 이쪽은 Attention에도 MoE를 적용했기에 동등한 비교라기에는 좀 어려울 수 있겠네요. 이전의 연구에서도 (https://arxiv.org/abs/2406.06248) Structured Matrix로 더 나은 결과를 얻기는 어려웠던 것 같습니다.

<english>
Combining the methods that uses structured matrices like Tensor Train into einsum and estimated scaling law. For the result, there was no methods that improves upon the method uses dense matrices. For MoEs Block Tensor Train showed slightly better results, but in this case they applied MoE into Attention, so it is hard to say that it was fair comparision. Previous research (https://arxiv.org/abs/2406.06248) also showed that it is hard to get better results with structured matrices.
</english>

#efficient-training #scaling-law

# Links

[[240610 Compute Better Spent.md]]