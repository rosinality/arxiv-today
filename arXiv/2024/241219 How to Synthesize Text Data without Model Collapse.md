https://arxiv.org/abs/2412.14689

*How to Synthesize Text Data without Model Collapse?* (Xuekai Zhu, Daixuan Cheng, Hengli Li, Kaiyan Zhang, Ermo Hua, Xingtai Lv, Ning Ding, Zhouhan Lin, Zilong Zheng, Bowen Zhou)

> Model collapse in synthetic data indicates that iterative training on self-generated data leads to a gradual decline in performance. With the proliferation of AI models, synthetic data will fundamentally reshape the web data ecosystem. Future GPT-$\{n\}$ models will inevitably be trained on a blend of synthetic and human-produced data. In this paper, we focus on two questions: what is the impact of synthetic data on language model training, and how to synthesize data without model collapse? We first pre-train language models across different proportions of synthetic data, revealing a negative correlation between the proportion of synthetic data and model performance. We further conduct statistical analysis on synthetic data to uncover distributional shift phenomenon and over-concentration of n-gram features. Inspired by the above findings, we propose token editing on human-produced data to obtain semi-synthetic data. As a proof of concept, we theoretically demonstrate that token-level editing can prevent model collapse, as the test error is constrained by a finite upper bound. We conduct extensive experiments on pre-training from scratch, continual pre-training, and supervised fine-tuning. The results validate our theoretical proof that token-level editing improves data quality and enhances model performance.

합성 데이터가 커버하는 분포의 범위가 좁다는 문제에 대한 분석. 이에 대한 대안으로 사람이 생성한 데이터에 대해 확률이 높은 토큰을 다른 토큰으로 교체하는 형태의 데이터 생성 방법을 제안했습니다.

합성 데이터를 사용할 것인가 자체보다는 어떻게 합성 데이터를 생성하는 것이 좋은가의 문제로 넘어가야 할 시점이네요.

<english>
Analysis on the problem of converage of distribution of synthetic data is narrow. Alternatively, they devised method to synthesize the data that replacing tokens with high probability in human generated texts into another tokens.

I think it is point to discuss how we should generate synthetic data, rather than whether we should use it or not.
</english>

#synthetic-data 