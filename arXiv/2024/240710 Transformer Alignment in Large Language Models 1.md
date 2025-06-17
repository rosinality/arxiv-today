https://arxiv.org/abs/2407.07810

*Transformer Alignment in Large Language Models* (Murdock Aubry, Haoming Meng, Anton Sugolov, Vardan Papyan)

> Large Language Models (LLMs) have made significant strides in natural language processing, and a precise understanding of the internal mechanisms driving their success is essential. We regard LLMs as transforming embeddings via a discrete, coupled, nonlinear, dynamical system in high dimensions. This perspective motivates tracing the trajectories of individual tokens as they pass through transformer blocks, and linearizing the system along these trajectories through their Jacobian matrices. In our analysis of 38 openly available LLMs, we uncover the alignment of top left and right singular vectors of Residual Jacobians, as well as the emergence of linearity and layer-wise exponential growth. Notably, we discover that increased alignment positively correlates with model performance. Metrics evaluated post-training show significant improvement in comparison to measurements made with randomly initialized weights, highlighting the significant effects of training in transformers. These findings reveal a remarkable level of regularity that has previously been overlooked, reinforcing the dynamical interpretation and paving the way for deeper understanding and optimization of LLM architectures.

트랜스포머 블록의 야코비안의 Singular Vector들이 서로 다른 레이어의 Singular Vector들과 정렬되어 있다는 결과. 더 나아가서 더 잘 학습된 모델일수록 더 잘 정렬되어 있다는 추정. (이 효과는 좀 약한 것 같긴 합니다만.) 뭔가 초기화를 잘 하면 이런 정렬을 임의로 유도할 수도 있지 않을까요.

#transformer 