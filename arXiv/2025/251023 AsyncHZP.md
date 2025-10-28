https://arxiv.org/abs/2510.20111

*AsyncHZP: Hierarchical ZeRO Parallelism with Asynchronous Scheduling for Scalable LLM Training* (Huawei Bai, Yifan Huang, Wenqi Shi, Ansheng You, Feifan Shao, Tengfei Han, Minghui Yu)

> The training efficiency and scalability of language models on massive clusters currently remain a critical bottleneck. Mainstream approaches like ND parallelism are often cumbersome and complex, while flexible alternatives such as the Zero Redundancy Optimizer (ZeRO) are frequently hampered by communication overhead. In this paper, we propose Asynchronous Hierarchical Zero Parallelism (AsyncHZP), a novel asynchronous variant of ZeRO designed to achieve superior performance while maintaining simplicity and memory efficiency. Unlike traditional ZeRO, which employs over-fine-grained sharding that can lead to inefficient communication, AsyncHZP adaptively reshards parameters, gradients, and optimizer states across different replica groups. This strategy optimizes device memory utilization and significantly reduces communication overhead. In addition, we also design a multi-stream asynchronous scheduling method that executes parameter all-gather and gradient reduce-scatter operations in dedicated background threads, effectively overlapping communication with computation while incurring negligible memory fragmentation. Empirical evaluations on both Dense and Mixture-of-Experts (MoE) models confirm that AsyncHZP maintains robust stability at scale. It consistently outperforms classic ND parallelism, achieving state-of-the-art performance without complex strategic tuning, thereby simplifying the path to efficient large-scale training.

ZeRO-1/2/3의 샤딩을 디커플링. CP, PP와 잘 결합하는 것이 가능.

Decouples sharding of ZeRO-1/2/3 from each other. It allows to well combined with CP and TP.

#parallelism 