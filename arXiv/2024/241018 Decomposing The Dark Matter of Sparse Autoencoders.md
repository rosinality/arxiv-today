https://arxiv.org/abs/2410.14670

*Decomposing The Dark Matter of Sparse Autoencoders* (Joshua Engels, Logan Riggs, Max Tegmark)

> Sparse autoencoders (SAEs) are a promising technique for decomposing language model activations into interpretable linear features. However, current SAEs fall short of completely explaining model performance, resulting in "dark matter": unexplained variance in activations. This work investigates dark matter as an object of study in its own right. Surprisingly, we find that much of SAE dark matter--about half of the error vector itself and >90% of its norm--can be linearly predicted from the initial activation vector. Additionally, we find that the scaling behavior of SAE error norms at a per token level is remarkably predictable: larger SAEs mostly struggle to reconstruct the same contexts as smaller SAEs. We build on the linear representation hypothesis to propose models of activations that might lead to these observations, including postulating a new type of "introduced error"; these insights imply that the part of the SAE error vector that cannot be linearly predicted ("nonlinear" error) might be fundamentally different from the linearly predictable component. To validate this hypothesis, we empirically analyze nonlinear SAE error and show that 1) it contains fewer not yet learned features, 2) SAEs trained on it are quantitatively worse, 3) it helps predict SAE per-token scaling behavior, and 4) it is responsible for a proportional amount of the downstream increase in cross entropy loss when SAE activations are inserted into the model. Finally, we examine two methods to reduce nonlinear SAE error at a fixed sparsity: inference time gradient pursuit, which leads to a very slight decrease in nonlinear error, and linear transformations from earlier layer SAE outputs, which leads to a larger reduction.

Sparse Autoencoder의 Irreducible Error에 대한 분석. 흥미로운 것은 오차의 상당 부분의 분산이 Feature에 대한 Linear Projection으로 예측이 가능하다는 것이네요. 이런 Irreducible Error가 해석의 측면에서 갖는 의미가 무엇일까요.

<english>
Analysis on irreducible error of sparse autoencoder. Interesting point is that large portion of error variances can be explained by linear projection of features. What would be the meaning of these irreducible errors on interpretation?
</english>

#mechanistic-interpretation