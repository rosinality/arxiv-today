https://arxiv.org/abs/2402.07871

*Scaling Laws for Fine-Grained Mixture of Experts* (Jakub Krajewski, Jan Ludziejewski, Kamil Adamczewski, Maciej Pióro, Michał Krutul, Szymon Antoniak, Kamil Ciebiera, Krystian Król, Tomasz Odrzygóźdź, Piotr Sankowski, Marek Cygan, Sebastian Jaszczur)

> Mixture of Experts (MoE) models have emerged as a primary solution for reducing the computational cost of Large Language Models. In this work, we analyze their scaling properties, incorporating an expanded range of variables. Specifically, we introduce a new hyperparameter, granularity, whose adjustment enables precise control over the size of the experts. Building on this, we establish scaling laws for fine-grained MoE, taking into account the number of training tokens, model size, and granularity. Leveraging these laws, we derive the optimal training configuration for a given computational budget. Our findings not only show that MoE models consistently outperform dense Transformers but also highlight that the efficiency gap between dense and MoE models widens as we scale up the model size and training budget. Furthermore, we demonstrate that the common practice of setting the size of experts in MoE to mirror the feed-forward layer is not optimal at almost any computational budget.

MoE 모델에 대한 Scaling Law가 있었지만 (https://arxiv.org/abs/2202.01169) 이는 고정된 토큰에 대한 결과였죠. 여기서는 학습 토큰 수와 함께 Granularity, 즉 Expert의 히든 차원의 크기를 축소하는 요인까지 고려한 Scaling Law를 만들었습니다. DeepSeekMoE (https://arxiv.org/abs/2401.06066) 와 비슷한 세팅이라고 볼 수 있겠습니다.

Expert의 숫자 요인이 빠져 있고 실험의 규모가 좀 작다는 것이 아쉽기는 한데 선례도 있으니 MoE 디자인에서 고려할만한 부분이겠다 싶네요.

#moe #scaling-law 

Previously study on scaling law MoE was done, but it is result from fixed training token budgets. In this study authors consider scaling law with number of tokens, and granularity, that is, factor that reducing hidden dimensions for each experts. It is configuration similar to DeepSeekMoE.

For limitations, scaling law of this paper does not include number of experts factor, and overall scale of experiments are rather small. But as there are previous approaches with varying granularity, I think it is beneficial to consider this dimension in designing MoE models.

# Links

[[220202 Unified Scaling Laws for Routed Language Models.md]]
[[240111 DeepSeekMoE.md]]