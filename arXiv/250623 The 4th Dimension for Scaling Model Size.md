https://arxiv.org/abs/2506.18233

*The 4th Dimension for Scaling Model Size* (Ruike Zhu, Hanwen Zhang, Tianyu Shi, Chi Wang, Tianyi Zhou, Zengyi Qin)

> Scaling the size of large language models typically involves three dimensions: depth, width, and the number of parameters. In this work, we explore a fourth dimension, virtual logical depth (VLD), which increases the effective algorithmic depth without changing the overall parameter count by reusing parameters within the model. Although parameter reuse is not a new concept, its potential and characteristics in model scaling have not been thoroughly studied. Through carefully designed controlled experiments, we make the following key discoveries regarding VLD scaling: VLD scaling forces the knowledge capacity of the model to remain almost constant, with only minor variations. VLD scaling enables a significant improvement in reasoning capability, provided the scaling method is properly implemented. The number of parameters correlates with knowledge capacity, but not with reasoning capability. Under certain conditions, it is not necessary to increase the parameter count to enhance reasoning. These findings are consistent across various model configurations and are likely to be generally valid within the scope of our experiments.

레이어 재사용으로 모델을 확장했을 때 저장하는 정보의 양은 고정하면서 추론의 능력을 향상시킬 수 있다는 연구.

#transformer 