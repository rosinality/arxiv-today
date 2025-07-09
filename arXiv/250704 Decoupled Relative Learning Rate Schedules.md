https://arxiv.org/abs/2507.03526

*Decoupled Relative Learning Rate Schedules* (Jan Ludziejewski, Jan Małaśnicki, Maciej Pióro, Michał Krutul, Kamil Ciebiera, Maciej Stefaniak, Jakub Krajewski, Piotr Sankowski, Marek Cygan, Kamil Adamczewski, Sebastian Jaszczur)

> In this work, we introduce a novel approach for optimizing LLM training by adjusting learning rates across weights of different components in Transformer models. Traditional methods often apply a uniform learning rate across all network layers, potentially overlooking the unique dynamics of each part. Remarkably, our introduced relative learning rates, RLRS, method accelerates the training process by up to $23\%$, particularly in complex models such as Mixture of Experts (MoE). Hyperparameters of RLRS can be efficiently tuned on smaller models and then effectively reused on models up to $27\times$ larger. This simple and effective method results in a substantial reduction in training time and computational resources, offering a practical and scalable solution for optimizing large-scale neural networks.

모듈마다 다른 LR 스케줄을 부여하자는 아이디어. 작은 모델에서 스케줄을 찾은 다음 큰 모델에 적용하는 간단한 방식입니다.

#optimization #moe 