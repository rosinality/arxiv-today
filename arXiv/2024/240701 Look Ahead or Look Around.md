https://arxiv.org/abs/2407.00935

*Look Ahead or Look Around? A Theoretical Comparison Between Autoregressive and Masked Pretraining* (Qi Zhang, Tianqi Du, Haotian Huang, Yifei Wang, Yisen Wang)

> In recent years, the rise of generative self-supervised learning (SSL) paradigms has exhibited impressive performance across visual, language, and multi-modal domains. While the varied designs of generative SSL objectives lead to distinct properties in downstream tasks, a theoretical understanding of these differences remains largely unexplored. In this paper, we establish the first theoretical comparisons between two leading generative SSL paradigms: autoregressive SSL and masked SSL. Through establishing theoretical frameworks, we elucidate the strengths and limitations of autoregressive and masked SSL within the primary evaluation tasks of classification and content generation. Our findings demonstrate that in classification tasks, the flexibility of targeted tokens in masked SSL fosters more inter-sample connections compared to the fixed position of target tokens in autoregressive SSL, which yields superior clustering performance. In content generation tasks, the misalignment between the flexible lengths of test samples and the fixed length of unmasked texts in masked SSL (vs. flexible lengths of conditional texts in autoregressive SSL) hinders its generation performance. To leverage each other's strengths and mitigate weaknesses, we propose diversity-enhanced autoregressive and variable-length masked objectives, which substantially improve the classification performance of autoregressive SSL and the generation performance of masked SSL. Code is available at https://github.com/PKU-ML/LookAheadLookAround.

Causal LM과 MLM Objective를 컨텍스트 토큰과 타겟 토큰의 Co-occurrence 행렬의 관점에서 분석. 이 행렬의 연결성이 MLM에서 더 높기 때문에 분류 과제 등에 대해 더 나은 성능을 나타낸다는 분석. 반대로 Causal LM이 생성 능력이 좋은 이유에 대한 분석도 있습니다. (학습과 테스트 시점의 길이 차이나 토큰의 위치에 따른 예측 변화 문제 등.)

이 문제에 대한 대응으로 Causal LM과 MLM Objective를 개선하는데 Causal LM에서는 Multi Token Prediction, MLM에서는 Prefix LM이나 Masked Diffusion 같은 형태의 마스크 비율을 다양화 하는 방식을 사용했습니다.

분류 과제 등에 대한 적용을 염두에 둔 것이긴 하지만 여러 토큰 예측 과제가 등장했다는 것이 흥미롭네요. (https://arxiv.org/abs/2403.06963, https://arxiv.org/abs/2404.19737) 추론 속도 가속에도 사용할 수 있으니 (https://arxiv.org/abs/2401.10774) 실험해보면 재미있는 접근일 것 같습니다.

#pretraining #self-supervision

# Links

[[240430 Better & Faster Large Language Models via Multi-token Prediction.md]]
[[240311 The pitfalls of next-token prediction.md]]