https://arxiv.org/abs/2511.11238

*Virtual Width Networks* (ByteDance Seed)

> We introduce Virtual Width Networks (VWN), a framework that delivers the benefits of wider representations without incurring the quadratic cost of increasing the hidden size. VWN decouples representational width from backbone width, expanding the embedding space while keeping backbone compute nearly constant. In our large-scale experiment, an 8-times expansion accelerates optimization by over 2 times for next-token and 3 times for next-2-token prediction. The advantage amplifies over training as both the loss gap grows and the convergence-speedup ratio increases, showing that VWN is not only token-efficient but also increasingly effective with scale. Moreover, we identify an approximately log-linear scaling relation between virtual width and loss reduction, offering an initial empirical basis and motivation for exploring virtual-width scaling as a new dimension of large-model efficiency.

블럭 크기 변경 없이 Hidden State의 크기 증대. 모두가 Skip Connection의 변형을 만들던 시절에서부터 시작된 고전적인 아이디어. 그렇지만 시도할 가치가 있을지도.

Expanding hidden states without increasing block dimensions. Classical line of approaches from the era when everyone tried to make variants of skip connections, but it could be worth trying.

#transformer 