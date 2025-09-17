https://arxiv.org/abs/2507.07101

*Small Batch Size Training for Language Models: When Vanilla SGD Works, and Why Gradient Accumulation Is Wasteful* (Martin Marek, Sanae Lotfi, Aditya Somasundaram, Andrew Gordon Wilson, Micah Goldblum)

> Conventional wisdom dictates that small batch sizes make language model pretraining and fine-tuning unstable, motivating gradient accumulation, which trades off the number of optimizer steps for a proportional increase in batch size. While it is common to decrease the learning rate for smaller batch sizes, other hyperparameters are often held fixed. In this work, we revisit small batch sizes all the way down to batch size one, and we propose a rule for scaling Adam hyperparameters to small batch sizes. We find that small batch sizes (1) train stably, (2) are consistently more robust to hyperparameter choices, (3) achieve equal or better per-FLOP performance than larger batch sizes, and (4) notably enable stable language model training with vanilla SGD, even without momentum, despite storing no optimizer state. Building on these results, we provide practical recommendations for selecting a batch size and setting optimizer hyperparameters. We further recommend against gradient accumulation unless training on multiple devices with multiple model replicas, bottlenecked by inter-device bandwidth.

작은 배치 크기에서는 SGD도 트랜스포머 LM 학습이 가능하다는 결과의 연장선이군요 (https://arxiv.org/abs/2506.12543). 여기서는 β_2를 조정해 Adam이 작은 배치 크기에서 잘 작동하게 만드는 실험을 했습니다.

<english>
A study that SGD can be used for transformer LM training when batch size is small, which is extension of previous research (https://arxiv.org/abs/2506.12543). This works shows that it is possible to make Adam works well in small batch sizes by adjusting β_2.
</english>

#optimization 