https://arxiv.org/abs/2505.05427

*Ultra-FineWeb: Efficient Data Filtering and Verification for High-Quality LLM Training Data* (Yudong Wang, Zixuan Fu, Jie Cai, Peijun Tang, Hongya Lyu, Yewei Fang, Zhi Zheng, Jie Zhou, Guoyang Zeng, Chaojun Xiao, Xu Han, Zhiyuan Liu)

> Data quality has become a key factor in enhancing model performance with the rapid development of large language models (LLMs). Model-driven data filtering has increasingly become a primary approach for acquiring high-quality data. However, it still faces two main challenges: (1) the lack of an efficient data verification strategy makes it difficult to provide timely feedback on data quality; and (2) the selection of seed data for training classifiers lacks clear criteria and relies heavily on human expertise, introducing a degree of subjectivity. To address the first challenge, we introduce an efficient verification strategy that enables rapid evaluation of the impact of data on LLM training with minimal computational cost. To tackle the second challenge, we build upon the assumption that high-quality seed data is beneficial for LLM training, and by integrating the proposed verification strategy, we optimize the selection of positive and negative samples and propose an efficient data filtering pipeline. This pipeline not only improves filtering efficiency, classifier quality, and robustness, but also significantly reduces experimental and inference costs. In addition, to efficiently filter high-quality data, we employ a lightweight classifier based on fastText, and successfully apply the filtering pipeline to two widely-used pre-training corpora, FineWeb and Chinese FineWeb datasets, resulting in the creation of the higher-quality Ultra-FineWeb dataset. Ultra-FineWeb contains approximately 1 trillion English tokens and 120 billion Chinese tokens. Empirical results demonstrate that the LLMs trained on Ultra-FineWeb exhibit significant performance improvements across multiple benchmark tasks, validating the effectiveness of our pipeline in enhancing both data quality and training efficiency.

여러 방법으로 전처리된 데이터를 시드로 설정한 다음 Llama 3 스타일을 따라 Decay 시점에 필터링된 데이터를 결합해 평가하는 사이클을 사용해 데이터를 필터링하는 방법.

데이터 품질 필터링은 중요한 요소죠. 다만 프리트레이닝의 규모가 점점 늘어나는 시점에서는 오히려 모델의 성능에 기여할 수 있는 텍스트 품질의 최저선은 무엇인가를 물을 필요가 있다고 봅니다.

<english>
Setup seeds from the data preprocessed by various way, and filter the data using the cycle by evaluating it combining filtered data at decay times, following Llama 3's method.

Quality filtering of data is crucial component. But as the scale of pretraining are increasing, maybe we need to ask what is the lowest line of text quality that can be benefit model performance.
</english>

#pretraining #corpus 