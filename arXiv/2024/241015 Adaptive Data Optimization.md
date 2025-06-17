https://arxiv.org/abs/2410.11820

*Adaptive Data Optimization: Dynamic Sample Selection with Scaling Laws* (Yiding Jiang, Allan Zhou, Zhili Feng, Sadhika Malladi, J. Zico Kolter)

> The composition of pretraining data is a key determinant of foundation models' performance, but there is no standard guideline for allocating a limited computational budget across different data sources. Most current approaches either rely on extensive experiments with smaller models or dynamic data adjustments that also require proxy models, both of which significantly increase the workflow complexity and computational overhead. In this paper, we introduce Adaptive Data Optimization (ADO), an algorithm that optimizes data distributions in an online fashion, concurrent with model training. Unlike existing techniques, ADO does not require external knowledge, proxy models, or modifications to the model update. Instead, ADO uses per-domain scaling laws to estimate the learning potential of each domain during training and adjusts the data mixture accordingly, making it more scalable and easier to integrate. Experiments demonstrate that ADO can achieve comparable or better performance than prior methods while maintaining computational efficiency across different computation scales, offering a practical solution for dynamically adjusting data distribution without sacrificing flexibility or increasing costs. Beyond its practical benefits, ADO also provides a new perspective on data collection strategies via scaling laws.

각 도메인에 대한 학습 Loss를 추정하는 Scaling Law를 사용해 데이터셋의 비율 결정. 재미있는 것은 각 도메인의 토큰 수의 비율로 비율을 설정하는 베이스라인이 상당히 강력하다는 것이네요.

<english>
Decide ratio of the dataset using scaling law that estimates training loss for each domain. Interestingly, baseline that set the ratio using number of tokens per domain is strong.
</english>

#scaling-law #dataset 