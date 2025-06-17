https://arxiv.org/abs/2502.05967

*$μ$nit Scaling: Simple and Scalable FP8 LLM Training* (Saaketh Narayan, Abhay Gupta, Mansheej Paul, Davis Blalock)

> Large Language Model training with 8-bit floating point (FP8) formats promises significant efficiency improvements, but reduced numerical precision makes training challenging. It is currently possible to train in FP8 only if one is willing to tune various hyperparameters, reduce model scale, or accept the overhead of computing dynamic scale factors. We demonstrate simple, scalable FP8 training that requires no dynamic scaling factors or special hyperparameters, even at large model sizes. Our method, $\mu$nit Scaling ($\mu$S), also enables simple hyperparameter transfer across model widths, matched numerics across training and inference, and other desirable properties. $\mu$nit Scaling is straightforward to implement, consisting of a set of minimal interventions based on a first-principles analysis of common transformer operations. We validate our method by training models from 1B to 13B parameters, performing all hidden linear layer computations in FP8. We achieve quality equal to higher precision baselines while also training up to 33% faster.

가변 Scaling factor 없이 FP8 학습을 하기 위한 방법.

<english>
A method for FP8 training without dynamic scaling factor.
</english>

#efficient-training 