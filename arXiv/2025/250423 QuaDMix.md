https://arxiv.org/abs/2504.16511

*QuaDMix: Quality-Diversity Balanced Data Selection for Efficient LLM Pretraining* (Fengze Liu, Weidong Zhou, Binbin Liu, Zhimiao Yu, Yifan Zhang, Haobin Lin, Yifeng Yu, Xiaohuan Zhou, Taifeng Wang, Yong Cao)

> Quality and diversity are two critical metrics for the training data of large language models (LLMs), positively impacting performance. Existing studies often optimize these metrics separately, typically by first applying quality filtering and then adjusting data proportions. However, these approaches overlook the inherent trade-off between quality and diversity, necessitating their joint consideration. Given a fixed training quota, it is essential to evaluate both the quality of each data point and its complementary effect on the overall dataset. In this paper, we introduce a unified data selection framework called QuaDMix, which automatically optimizes the data distribution for LLM pretraining while balancing both quality and diversity. Specifically, we first propose multiple criteria to measure data quality and employ domain classification to distinguish data points, thereby measuring overall diversity. QuaDMix then employs a unified parameterized data sampling function that determines the sampling probability of each data point based on these quality and diversity related labels. To accelerate the search for the optimal parameters involved in the QuaDMix framework, we conduct simulated experiments on smaller models and use LightGBM for parameters searching, inspired by the RegMix method. Our experiments across diverse models and datasets demonstrate that QuaDMix achieves an average performance improvement of 7.2% across multiple benchmarks. These results outperform the independent strategies for quality and diversity, highlighting the necessity and ability to balance data quality and diversity.

프리트레이닝 코퍼스의 품질과 다양성을 확보하려는 시도. 코퍼스에서 도메인을 나누고 각 도메인에 대해 품질 지표와 샘플링 비율을 모델 학습 실험을 통해 결정.

<english>
Attempt to ensure quality and diversity of pretraining corpus. After separate corpus into domains, determines quality metrics and sampling ratios for each domains using small scale model training experiments.
</english>

#pretraining #corpus 