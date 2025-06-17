https://arxiv.org/abs/2408.08310

*ScalingFilter: Assessing Data Quality through Inverse Utilization of Scaling Laws* (Ruihang Li, Yixuan Wei, Miaosen Zhang, Nenghai Yu, Han Hu, Houwen Peng)

> High-quality data is crucial for the pre-training performance of large language models. Unfortunately, existing quality filtering methods rely on a known high-quality dataset as reference, which can introduce potential bias and compromise diversity. In this paper, we propose ScalingFilter, a novel approach that evaluates text quality based on the perplexity difference between two language models trained on the same data, thereby eliminating the influence of the reference dataset in the filtering process. An theoretical analysis shows that ScalingFilter is equivalent to an inverse utilization of scaling laws. Through training models with 1.3B parameters on the same data source processed by various quality filters, we find ScalingFilter can improve zero-shot performance of pre-trained models in downstream tasks. To assess the bias introduced by quality filtering, we introduce semantic diversity, a metric of utilizing text embedding models for semantic representations. Extensive experiments reveal that semantic diversity is a reliable indicator of dataset diversity, and ScalingFilter achieves an optimal balance between downstream performance and semantic diversity.

DeepSeek LLM의 데이터 퀄리티가 향상될수록 Scaling Law에서 모델 크기에 대한 Exponent가 높아진다는 아이디어를 데이터 퀄리티 측정에 연결. 작은 모델과 큰 모델을 같은 데이터에 대해 학습시킨 다음 이 두 모델의 Perplexity의 비율이 퀄리티의 척도가 된다는 아이디어입니다.

이를 통해 데이터셋을 필터링하는데 사용합니다. 어떤 데이터에 대해 LM을 학습하는가가 필터링 성능에 영향을 미친다는 것을 고려하면 데이터셋의 유사도라는 측면도 있을 듯 한데 모델 크기에 따른 비율 차이를 고려한다는 것을 생각하면 Learnability와의 관계도 있을 듯 하네요. (https://arxiv.org/abs/2206.07137) 생각해볼만한 방법인 듯 합니다.

#scaling-law #corpus

# Links

