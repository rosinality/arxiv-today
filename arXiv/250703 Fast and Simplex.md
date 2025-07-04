https://arxiv.org/abs/2507.02754

*Fast and Simplex: 2-Simplicial Attention in Triton* (Aurko Roy, Timothy Chou, Sai Surya Duvvuri, Sijia Chen, Jiecao Yu, Xiaodong Wang, Manzil Zaheer, Rohan Anil)

> Recent work has shown that training loss scales as a power law with both model size and the number of tokens, and that achieving compute-optimal models requires scaling model size and token count together. However, these scaling laws assume an infinite supply of data and apply primarily in compute-bound settings. As modern large language models increasingly rely on massive internet-scale datasets, the assumption that they are compute-bound is becoming less valid. This shift highlights the need for architectures that prioritize token efficiency. In this work, we investigate the use of the 2-simplicial Transformer, an architecture that generalizes standard dot-product attention to trilinear functions through an efficient Triton kernel implementation. We demonstrate that the 2-simplicial Transformer achieves better token efficiency than standard Transformers: for a fixed token budget, similarly sized models outperform their dot-product counterparts on tasks involving mathematics, coding, reasoning, and logic. We quantify these gains by demonstrating that $2$-simplicial attention changes the exponent in the scaling laws for knowledge and reasoning tasks compared to dot product attention.

Trilinear Attention. 고전적인 아이디어가 다시 등장했네요. 연산 증가는 피할 수 없으니 Local Attention을 사용했습니다.

실험 세팅이 좀 특이합니다. Scaling Law 추정도 했는데 경사가 변화했군요. 추정치가 정확할지는 모르겠네요.

<english>
A trilinear attention. Classical idea is re-emerged. As it is not possible to avoid increase in computation, they used local attention.

Experimental setting is somewhat special. They also estimated scaling law, found slope is changed. But I wonder estimated value would be accurate.
</english>

#transformer #scaling-law 