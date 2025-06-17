https://arxiv.org/abs/2502.07827

*Implicit Language Models are RNNs: Balancing Parallelization and Expressivity* (Mark Schöne, Babak Rahmani, Heiner Kremer, Fabian Falck, Hitesh Ballani, Jannes Gladrow)

> State-space models (SSMs) and transformers dominate the language modeling landscape. However, they are constrained to a lower computational complexity than classical recurrent neural networks (RNNs), limiting their expressivity. In contrast, RNNs lack parallelization during training, raising fundamental questions about the trade off between parallelization and expressivity. We propose implicit SSMs, which iterate a transformation until convergence to a fixed point. Theoretically, we show that implicit SSMs implement the non-linear state-transitions of RNNs. Empirically, we find that only approximate fixed-point convergence suffices, enabling the design of a scalable training curriculum that largely retains parallelization, with full convergence required only for a small subset of tokens. Our approach demonstrates superior state-tracking capabilities on regular languages, surpassing transformers and SSMs. We further scale implicit SSMs to natural language reasoning tasks and pretraining of large-scale language models up to 1.3B parameters on 207B tokens - representing, to our knowledge, the largest implicit model trained to date. Notably, our implicit models outperform their explicit counterparts on standard benchmarks.

State Space Model의 표현력 제약을 Equilibrium Model로 해소. 얼마 전에도 Universal Transformer가 등장했었죠. (https://arxiv.org/abs/2502.05171) 이쪽 연구가 다시 나올지도 모르겠네요.

<english>
Relaxing the limitation of representation capacity of state space models using equilibrium models. Universal transformer also appeared recently (https://arxiv.org/abs/2502.05171). Maybe more studies in this direction would appear in the future.
</english>

#state-space-model

# Links

[[250207 Scaling up Test-Time Compute with Latent Reasoning.md]]