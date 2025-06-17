https://arxiv.org/abs/2506.10972

*Farseer: A Refined Scaling Law in Large Language Models* (Houyi Li, Wenzhen Zheng, Qiufeng Wang, Zhenyu Ding, Haoying Wang, Zili Wang, Shijie Xuyang, Ning Ding, Shuigeng Zhou, Xiangyu Zhang, Daxin Jiang)

> Training Large Language Models (LLMs) is prohibitively expensive, creating a critical scaling gap where insights from small-scale experiments often fail to transfer to resource-intensive production systems, thereby hindering efficient innovation. To bridge this, we introduce Farseer, a novel and refined scaling law offering enhanced predictive accuracy across scales. By systematically constructing a model loss surface $L(N,D)$, Farseer achieves a significantly better fit to empirical data than prior laws (e.g., Chinchilla's law). Our methodology yields accurate, robust, and highly generalizable predictions, demonstrating excellent extrapolation capabilities, improving upon Chinchilla's law by reducing extrapolation error by 433\%. This allows for the reliable evaluation of competing training strategies across all $(N,D)$ settings, enabling conclusions from small-scale ablation studies to be confidently extrapolated to predict large-scale performance. Furthermore, Farseer provides new insights into optimal compute allocation, better reflecting the nuanced demands of modern LLM training. To validate our approach, we trained an extensive suite of approximately 1,000 LLMs across diverse scales and configurations, consuming roughly 3 million NVIDIA H100 GPU hours. We are comprehensively open-sourcing all models, data, results, and logs at https://github.com/Farseer-Scaling-Law/Farseer to foster further research.

굉장한 결과네요. Chinchilla의 Parametric Model을 개선했습니다. Chinchilla Law의 의문스러운 부분이었던 모델 크기와 데이터 사이의 상호작용이 없다는 것을 개선했네요.

훨씬 정확하고 최적 데이터/모델 크기 비율이 연산량 증가에 따라 같이 증가한다는 것을 밝혔습니다.

<english>
Impressive result. This paper improves parametric model from Chinchilla. This work improved questioning choice of chinchilla law of it is not includes interaction between number of parameters and data sizes.

It is much more accurate, and it shows that optimal data to model size ratio increase with increased computes.
</english>

#scaling-law 