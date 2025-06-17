https://arxiv.org/abs/2410.08527

*Scaling Laws for Predicting Downstream Performance in LLMs* (Yangyi Chen, Binxuan Huang, Yifan Gao, Zhengyang Wang, Jingfeng Yang, Heng Ji)

> Precise estimation of downstream performance in large language models (LLMs) prior to training is essential for guiding their development process. Scaling laws analysis utilizes the statistics of a series of significantly smaller sampling language models (LMs) to predict the performance of the target LLM. For downstream performance prediction, the critical challenge lies in the emergent abilities in LLMs that occur beyond task-specific computational thresholds. In this work, we focus on the pre-training loss as a more computation-efficient metric for performance estimation. Our two-stage approach consists of first estimating a function that maps computational resources (e.g., FLOPs) to the pre-training Loss using a series of sampling models, followed by mapping the pre-training loss to downstream task Performance after the critical "emergent phase". In preliminary experiments, this FLP solution accurately predicts the performance of LLMs with 7B and 13B parameters using a series of sampling LMs up to 3B, achieving error margins of 5% and 10%, respectively, and significantly outperforming the FLOPs-to-Performance approach. This motivates FLP-M, a fundamental approach for performance prediction that addresses the practical need to integrate datasets from multiple sources during pre-training, specifically blending general corpora with code data to accurately represent the common necessity. FLP-M extends the power law analytical function to predict domain-specific pre-training loss based on FLOPs across data sources, and employs a two-layer neural network to model the non-linear relationship between multiple domain-specific loss and downstream performance. By utilizing a 3B LLM trained on a specific ratio and a series of smaller sampling LMs, FLP-M can effectively forecast the performance of 3B and 7B LLMs across various data mixtures for most benchmarks within 10% error margins.

도메인에 대한 Loss의 Scaling Law와 도메인 Loss를 사용한 벤치마크 점수 예측을 조합하여 벤치마크에 대한 Scaling Law를 구성. 과거 벤치마크에 대한 Scaling Law 추정을 시도한 작업들과 (https://arxiv.org/abs/2403.08540, https://arxiv.org/abs/2404.09937) 비슷한 점이 있습니다.

<english>
Constructing scaling law for benchmark by composing scaling law for domain loss, and predicting benchmark scores with domain loss. There are similar points with previous works tried to estimating scaling law for benchmarks. (https://arxiv.org/abs/2403.08540, https://arxiv.org/abs/2404.09937)
</english>

#scaling-law

# Links

[[240415 Compression Represents Intelligence Linearly.md]]
[[240313 Language models scale reliably with over-training and on downstream tasks.md]]