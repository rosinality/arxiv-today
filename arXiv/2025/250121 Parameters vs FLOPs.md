https://arxiv.org/abs/2501.12370

*Parameters vs FLOPs: Scaling Laws for Optimal Sparsity for Mixture-of-Experts Language Models* (Samira Abnar, Harshay Shah, Dan Busbridge, Alaaeldin Mohamed Elnouby Ali, Josh Susskind, Vimal Thilak)

> Scaling the capacity of language models has consistently proven to be a reliable approach for improving performance and unlocking new capabilities. Capacity can be primarily defined by two dimensions: the number of model parameters and the compute per example. While scaling typically involves increasing both, the precise interplay between these factors and their combined contribution to overall capacity remains not fully understood. We explore this relationship in the context of sparse Mixture-of-Expert models (MoEs), which allow scaling the number of parameters without proportionally increasing the FLOPs per example. We investigate how varying the sparsity level, i.e., the ratio of non-active to total parameters, affects model performance in terms of both pretraining and downstream performance. We find that under different constraints (e.g. parameter size and total training compute), there is an optimal level of sparsity that improves both training efficiency and model performance. These results provide a better understanding of the impact of sparsity in scaling laws for MoEs and complement existing works in this area, offering insights for designing more efficient architectures.

MoE의 Sparsity에 대한 Scaling Law. 모델 크기에 따라 Sparsity가 증가하는 것이 Compute Optimal이라는 결론입니다. 사실 최근 MoE 모델들은 이 논문에서 정의한 Sparsity가 (Routed Expert의 수) 꽤 높은 편이긴 하죠. 물론 FLOPs만 고려했을 때의 이야기이긴 합니다.

<english>
Scaling law for sparsity in MoE. The result says it is compute optimal to increase sparsity along with model sizes. Actually recent MoE models have quite high sparsity defined in this paper (number of routed experts). Of course this conclusions are valid when considering FLOPs only.
</english>

#moe #scaling-law #sparsity 