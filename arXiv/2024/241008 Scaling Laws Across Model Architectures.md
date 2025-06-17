https://arxiv.org/abs/2410.05661

*Scaling Laws Across Model Architectures: A Comparative Analysis of Dense and MoE Models in Large Language Models* (Siqi Wang, Zhengyu Chen, Bei Li, Keqing He, Min Zhang, Jingang Wang)

> The scaling of large language models (LLMs) is a critical research area for the efficiency and effectiveness of model training and deployment. Our work investigates the transferability and discrepancies of scaling laws between Dense Models and Mixture of Experts (MoE) models. Through a combination of theoretical analysis and extensive experiments, including consistent loss scaling, optimal batch size and learning rate scaling, and resource allocation strategies scaling, our findings reveal that the power-law scaling framework also applies to MoE Models, indicating that the fundamental principles governing the scaling behavior of these models are preserved, even though the architecture differs. Additionally, MoE Models demonstrate superior generalization, resulting in lower testing losses with the same training compute budget compared to Dense Models. These findings indicate the scaling consistency and transfer generalization capabilities of MoE Models, providing new insights for optimizing MoE Model training and deployment strategies.

MoE에 대한 Scaling Law. 최적 모델 규모에 대해서는 MoE 모델이 Dense 모델보다 지수가 더 크네요. (더 큰 모델 규모를 선호.) 최적 LR과 배치 크기에 대한 Scaling Law에 대해서는 본문에서는 차이가 있다고 하는데 Loss 타겟에 대해서는 사실 꽤 비슷한 것 같습니다. 모델 규모에 대해서는 차이가 있는 듯 하지만 그래프만으로는 알기 어렵네요.

<english>
Scaling law for MoE. In optimal model scales MoE has larger exponent compared to dense models. (That means, prefer larger models.) For optimal LR and batch size scaling laws, the paper suggest that there is differences, but I think it is quite similar with respect to specific LR targets. Maybe there exists differences along with model scales, but it is hard to know it from the plots.
</english>

#scaling-law #moe 