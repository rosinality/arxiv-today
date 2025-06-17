https://arxiv.org/abs/2503.10537

*Structured Preconditioners in Adaptive Optimization: A Unified Analysis* (Shuo Xie, Tianhao Wang, Sashank Reddi, Sanjiv Kumar, Zhiyuan Li)

> We present a novel unified analysis for a broad class of adaptive optimization algorithms with structured (e.g., layerwise, diagonal, and kronecker-factored) preconditioners for both online regret minimization and offline convex optimization. Our analysis not only provides matching rate to several important structured preconditioned algorithms including diagonal AdaGrad, full-matrix AdaGrad, and AdaGrad-Norm, but also gives an improved convergence rate for a one-sided variant of Shampoo over that of original Shampoo. Interestingly, more structured preconditioners (e.g., diagonal Adagrad, AdaGrad-Norm which use less space and compute) are often presented as computationally efficient approximations to full-matrix Adagrad, aiming for improved optimization performance through better approximations. Our unified analysis challenges this prevailing view and reveals, perhaps surprisingly, that more structured preconditioners, despite using less space and computation per step, can outperform their less structured counterparts. To demonstrate this, we show that one-sided Shampoo, which is relatively much cheaper than full-matrix AdaGrad could outperform it both theoretically and experimentally.

One-sided Shampoo 같은 구조를 더 부여한 Preconditioner가 Full-matrix Adagrad 같은 원 방법보다 오히려 더 나은 수렴률을 가질 수 있다는 분석.

The analysis suggests that a more structured preconditioner such as one-sided shampoo can achieve better convergence rates than "original" method like full-matrix adagrad.

#optimizer 