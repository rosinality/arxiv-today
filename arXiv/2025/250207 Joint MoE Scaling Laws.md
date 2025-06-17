https://arxiv.org/abs/2502.05172

*Joint MoE Scaling Laws: Mixture of Experts Can Be Memory Efficient* (Jan Ludziejewski, Maciej Pióro, Jakub Krajewski, Maciej Stefaniak, Michał Krutul, Jan Małaśnicki, Marek Cygan, Piotr Sankowski, Kamil Adamczewski, Piotr Miłoś, Sebastian Jaszczur)

> Mixture of Experts (MoE) architectures have significantly increased computational efficiency in both research and real-world applications of large-scale machine learning models. However, their scalability and efficiency under memory constraints remain relatively underexplored. In this work, we present joint scaling laws for dense and MoE models, incorporating key factors such as the number of active parameters, dataset size, and the number of experts. Our findings provide a principled framework for selecting the optimal MoE configuration under fixed memory and compute budgets. Surprisingly, we show that MoE models can be more memory-efficient than dense models, contradicting conventional wisdom. To derive and validate the theoretical predictions of our scaling laws, we conduct over 280 experiments with up to 2.7B active parameters and up to 5B total parameters. These results offer actionable insights for designing and deploying MoE models in practical large-scale training scenarios.

MoE Scaling Law. 이전에 나온 MoE Scaling Law와 맞춰보면 재미있습니다. (https://arxiv.org/abs/2410.05661) 이쪽에서는 고정 연산량에서 Expert의 수를 증가시켰을 때 Optimal Activated Weight와 토큰량에 집중하고 있네요. 여전히 MoE가 Activated Weight에 대한 Exponent가 크다는 것은 같습니다.

<english>
Scaling law for MoE. It is interesting when compared to previous trial on scaling law (https://arxiv.org/abs/2410.05661). This work focus on optimal activated weight and number of training tokens when number of experts increased for fixed computation budget. It is same that MoE has larger exponent on optimal activated weight per compute.
</english>

#scaling-law #moe

# Links

[[241008 Scaling Laws Across Model Architectures.md]]