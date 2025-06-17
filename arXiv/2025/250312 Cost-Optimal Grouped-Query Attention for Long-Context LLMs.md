https://arxiv.org/abs/2503.09579

*Cost-Optimal Grouped-Query Attention for Long-Context LLMs* (Yingfa Chen, Yutong Wu, Xu Han, Zhiyuan Liu, Maosong Sun)

> Building effective and efficient Transformer-based large language models (LLMs) has recently become a research focus, requiring maximizing model language capabilities and minimizing training and deployment costs. Existing efforts have primarily described complex relationships among model performance, parameter size, and data size, as well as searched for the optimal compute allocation to train LLMs. However, they overlook the impacts of context length and attention head configuration (the number of query and key-value heads in grouped-query attention) on training and inference. In this paper, we systematically compare models with different parameter sizes, context lengths, and attention head configurations in terms of model performance, computational cost, and memory cost. Then, we extend the existing scaling methods, which are based solely on parameter size and training compute, to guide the construction of cost-optimal LLMs during both training and inference. Our quantitative scaling studies show that, when processing sufficiently long sequences, a larger model with fewer attention heads can achieve a lower loss while incurring lower computational and memory costs. Our findings provide valuable insights for developing practical LLMs, especially in long-context processing scenarios. We will publicly release our code and data.

Attention 헤드의 수를 임베딩 차원과 분리해서 Attention 헤드의 수와 모델 크기 사이에서 최적 지점을 찾으려는 시도. 실제로 GQA의 크기, Window Attention의 비율 등은 이미 중요한 문제가 된 것 같습니다.

<english>
Attempt to find optimal points among number of attention heads and model sizes by decouple number of heads from embedding dimensions. Actually size of GQA, ratio of window attention is already became an important problem.
</english>

#scaling-law #transformer 