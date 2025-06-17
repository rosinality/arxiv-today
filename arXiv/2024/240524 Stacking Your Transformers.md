https://arxiv.org/abs/2405.15319

*Stacking Your Transformers: A Closer Look at Model Growth for Efficient LLM Pre-Training* (Wenyu Du, Tongxu Luo, Zihan Qiu, Zeyu Huang, Yikang Shen, Reynold Cheng, Yike Guo, Jie Fu)

> LLMs are computationally expensive to pre-train due to their large scale. Model growth emerges as a promising approach by leveraging smaller models to accelerate the training of larger ones. However, the viability of these model growth methods in efficient LLM pre-training remains underexplored. This work identifies three critical Obstacles: (O1) lack of comprehensive evaluation, (O2) untested viability for scaling, and (O3) lack of empirical guidelines. To tackle O1, we summarize existing approaches into four atomic growth operators and systematically evaluate them in a standardized LLM pre-training setting. Our findings reveal that a depthwise stacking operator, called Gstack, exhibits remarkable acceleration in training, leading to decreased loss and improved overall performance on eight standard NLP benchmarks compared to strong baselines. Motivated by these promising results, we conduct extensive experiments to delve deeper into Gstack to address O2 and O3. For O2 (untested scalability), our study shows that Gstack is scalable and consistently performs well, with experiments up to 7B LLMs after growth and pre-training LLMs with 750B tokens. For example, compared to a conventionally trained 7B model using 300B tokens, our Gstack model converges to the same loss with 194B tokens, resulting in a 54.6% speedup. We further address O3 (lack of empirical guidelines) by formalizing guidelines to determine growth timing and growth factor for Gstack, making it practical in general LLM pre-training. We also provide in-depth discussions and comprehensive ablation studies of Gstack. Our code and pre-trained model are available at https://llm-stacking.github.io/.

Layer Stacking, 즉 학습하던 모델의 레이어를 복붙해서 크기를 키운 다음 학습하는 방법이 효과적이라는 결과. 어느 시점에서 얼마나 모델을 키워야 하는지도 Scalign Law를 사용해 추정했습니다.

흥미로운 점은 Stacking을 하는 시점이 상당히 학습 초반이라는 점이네요. 모델이 클수록 뒤로 미뤄지지만 10 - 20B 정도의 지점입니다. 뭔가 좋은 Initialization을 해주는 효과라는 느낌이네요.

한 가지 더 흥미로운 점은 Function Preserving Transform이 더 효과적이지는 않았다는 점입니다. 직관적으로도 기존에 학습한 함수를 그대로 이어받는 것보다는 노이즈로 리셋해주는 쪽이 나을 수 있겠다 싶습니다.

이 계통 연구가 No Train No Gain (https://arxiv.org/abs/2307.06440) 덕에 그동안 인기가 없었던 듯 한데 (물론 이 논문에서도 그나마 가장 효과적인 것은 Layer Stacking이라고 하긴 합니다) 된다는 결과처럼 안 된다는 결과도 주의할 필요가 있다는 교훈이 될 수 있지 않을까 싶습니다.

#efficient-training #llm #scaling-law

# Links

[[230712 No Train No Gain.md]]