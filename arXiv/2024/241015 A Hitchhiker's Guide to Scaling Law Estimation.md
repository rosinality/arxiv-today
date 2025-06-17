https://arxiv.org/abs/2410.11840

*A Hitchhiker's Guide to Scaling Law Estimation* (Leshem Choshen, Yang Zhang, Jacob Andreas)

> Scaling laws predict the loss of a target machine learning model by extrapolating from easier-to-train models with fewer parameters or smaller training sets. This provides an efficient way for practitioners and researchers alike to compare pretraining decisions involving optimizers, datasets, and model architectures. Despite the widespread use of scaling laws to model the dynamics of language model training, there has been little work on understanding how to best estimate and interpret them. We collect (and release) a large-scale dataset containing losses and downstream evaluations for 485 previously published pretrained models. We use these to estimate more than 1000 scaling laws, then derive a set of best practices for estimating scaling laws in new model families. We find that fitting scaling laws to intermediate checkpoints of training runs (and not just their final losses) substantially improves accuracy, and that -- all else equal -- estimates of performance are generally most accurate when derived from other models of similar sizes. However, because there is a significant degree of variability across model seeds, training multiple small models is sometimes more useful than training a single large one. Moreover, while different model families differ scaling behavior, they are often similar enough that a target model's behavior can be predicted from a single model with the same architecture, along with scaling parameter estimates derived from other model families.

Scaling Law를 효율적으로 추정할 수 있는 방법들에 대한 고찰. 예를 들어 학습 중간 체크포인트도 추정에 사용하는 것이 오히려 더 정확하다 같은 탐색입니다.

<english>
Study on estimating scaling law efficiently. For example, this study explores that using intermediate checkpoint is beneficial for accuracy.
</english>

#scaling-law 