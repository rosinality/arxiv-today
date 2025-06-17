https://arxiv.org/abs/2404.02258

*Mixture-of-Depths: Dynamically allocating compute in transformer-based language models* (David Raposo, Sam Ritter, Blake Richards, Timothy Lillicrap, Peter Conway Humphreys, Adam Santoro)

> Transformer-based language models spread FLOPs uniformly across input sequences. In this work we demonstrate that transformers can instead learn to dynamically allocate FLOPs (or compute) to specific positions in a sequence, optimising the allocation along the sequence for different layers across the model depth. Our method enforces a total compute budget by capping the number of tokens ($k$) that can participate in the self-attention and MLP computations at a given layer. The tokens to be processed are determined by the network using a top-$k$ routing mechanism. Since $k$ is defined a priori, this simple procedure uses a static computation graph with known tensor sizes, unlike other conditional computation techniques. Nevertheless, since the identities of the $k$ tokens are fluid, this method can expend FLOPs non-uniformly across the time and model depth dimensions. Thus, compute expenditure is entirely predictable in sum total, but dynamic and context-sensitive at the token-level. Not only do models trained in this way learn to dynamically allocate compute, they do so efficiently. These models match baseline performance for equivalent FLOPS and wall-clock times to train, but require a fraction of the FLOPs per forward pass, and can be upwards of 50\% faster to step during post-training sampling.

Adaptive Depth / Early Exit과 비슷한데 연산을 레이어 중간에서 끊는 것이 아니라 각 레이어가 사용할 토큰의 양을 줄이는 방식이군요. 예를 들어 Self Attention이나 MLP가 시퀀스 내의 토큰 50%만 사용하도록 하고, Router를 사용해서 Top-K개를 끊어 레이어를 적용하는 방식입니다.

다만 Autoregressive Generation 상황이 문제겠군요. 일단은 성능 문제는 그렇게 크지 않다고 합니다.

#moe 