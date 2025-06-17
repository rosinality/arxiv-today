https://arxiv.org/abs/2502.17405

*Function-Space Learning Rates* (Edward Milsom, Ben Anson, Laurence Aitchison)

> We consider layerwise function-space learning rates, which measure the magnitude of the change in a neural network's output function in response to an update to a parameter tensor. This contrasts with traditional learning rates, which describe the magnitude of changes in parameter space. We develop efficient methods to measure and set function-space learning rates in arbitrary neural networks, requiring only minimal computational overhead through a few additional backward passes that can be performed at the start of, or periodically during, training. We demonstrate two key applications: (1) analysing the dynamics of standard neural network optimisers in function space, rather than parameter space, and (2) introducing FLeRM (Function-space Learning Rate Matching), a novel approach to hyperparameter transfer across model scales. FLeRM records function-space learning rates while training a small, cheap base model, then automatically adjusts parameter-space layerwise learning rates when training larger models to maintain consistent function-space updates. FLeRM gives hyperparameter transfer across model width, depth, initialisation scale, and LoRA rank in various architectures including MLPs with residual connections and transformers with different layer normalisation schemes.

작은 모델의 레이어의 출력의 변화를 기록하고 이 변화를 큰 모델 학습 시에 LR 조정에 사용한다는 아이디어.

<english>
Doing hyperparameter transformer by first recording output changes of small models and use it to adjust learning rate for larger model training.
</english>

#hyperparameter 