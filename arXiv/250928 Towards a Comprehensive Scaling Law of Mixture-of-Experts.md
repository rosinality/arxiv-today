https://arxiv.org/abs/2509.23678

*Towards a Comprehensive Scaling Law of Mixture-of-Experts* (Guoliang Zhao, Yuhan Fu, Shuaipeng Li, Xingwu Sun, Ruobing Xie, An Wang, Weidong Han, Zhen Yang, Weixuan Sun, Yudong Zhang, Cheng-zhong Xu, Di Wang, Jie Jiang)

> Mixture-of-Experts (MoE) models have become the consensus approach for enabling parameter-efficient scaling and cost-effective deployment in large language models. However, existing scaling laws for dense models are inapplicable to MoE models, which stems from three critical challenges: the multiplicity of influencing factors, their intricate coupling relationships and the non-monotonic nature of their performance impacts. They collectively necessitate a fine-grained investigation into MoE-specific scaling laws. In this work, we perform a systematic decomposition of MoE settings, identifying five key factors that influence model performance from both size and structural perspectives (data size ($D$), total model size ($N$), activated model size ($N_a$), number of active experts ($G$) and the ratio of shared experts ($S$)). Specifically, we design $446$ controlled experiments to characterize their marginal effects, ultimately constructing a comprehensive and precise joint MoE scaling law that considers all essential factors. Furthermore, we derive the theoretically optimal and practically efficiency-aware optimal configurations for $G$, $S$ and $N_a/N$ with detailed analyses. Our results demonstrate that the optimal settings for $G$ and $S$ are independent of both the model architecture and data size. With the scaling of $N$, the optimal activation parameter ratio of $N_a/N$ becomes sparser. Our proposed MoE scaling law could function as an accurate and insightful guidance to facilitate future MoE model design and training.

MoE Scaling Law. 이전 연구와 (https://arxiv.org/abs/2507.17702) 다른 점 중 하나는 여기서는 최적 Sparsity 비율이 있다고 주장한다는 것. (물론 공식의 형태 자체도 다르지만) 어쩌면 전체 Expert 중 Activate 되는 Expert의 비율이 아니라 전체 파라미터 중 Attention을 포함한 Activated 파라미터를 다루기 때문일지도.

GLM-4.5나 Qwen3 235B-A22B는 비교적 깊고 덜 Sparse한 구조를 채택. 어쩌면 좋은 디자인일지도?

MoE Scaling Law. One difference from previous research (https://arxiv.org/abs/2507.17702) is that this work claims there is an optimal sparsity ratio. This might be because this work considers total activated parameters (including attention) instead of the ratio of activated experts to total experts (Of course, the form of the formula itself is also different).

GLM-4.5 and Qwen 3 235B-A22B adopt relatively deeper and less sparse architectures - perhaps this could be a good design?

#moe #scaling-law 