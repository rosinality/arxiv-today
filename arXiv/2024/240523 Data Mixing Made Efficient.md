https://arxiv.org/abs/2405.14908

*Data Mixing Made Efficient: A Bivariate Scaling Law for Language Model Pretraining* (Ce Ge, Zhijian Ma, Daoyuan Chen, Yaliang Li, Bolin Ding)

> Large language models exhibit exceptional generalization capabilities, primarily attributed to the utilization of diversely sourced data. However, conventional practices in integrating this diverse data heavily rely on heuristic schemes, lacking theoretical guidance. This research tackles these limitations by investigating strategies based on low-cost proxies for data mixtures, with the aim of streamlining data curation to enhance training efficiency. Specifically, we propose a unified scaling law, termed BiMix, which accurately models the bivariate scaling behaviors of both data quantity and mixing proportions. We conduct systematic experiments and provide empirical evidence for the predictive power and fundamental principles of BiMix. Notably, our findings reveal that entropy-driven training-free data mixtures can achieve comparable or even better performance than more resource-intensive methods. We hope that our quantitative insights can shed light on further judicious research and development in cost-effective language modeling.

새삼스럽지만 LLM 튜닝의 정석은 Scaling Law 추정이군요. 학습 연산량과 데이터셋 비율에 따른 Scaling Law를 사용해 데이터셋의 비율을 설정했습니다.

그런데 사실 중간에 나오는 Conditional Entropy를 사용한 방법이 학습 없이도 잘 동작했다고 하네요.

여하간 각 데이터셋을 Scaling 했을 때의 가치와 퀄리티의 관계 등이 궁금했는데 그 부분에 대해 도움이 될 수 있을 듯 합니다.

#scaling-law #dataset 