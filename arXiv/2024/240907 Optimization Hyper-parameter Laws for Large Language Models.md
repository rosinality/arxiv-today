https://arxiv.org/abs/2409.04777

*Optimization Hyper-parameter Laws for Large Language Models* (Xingyu Xie, Kuangyu Ding, Shuicheng Yan, Kim-Chuan Toh, Tianwen Wei)

> Large Language Models have driven significant AI advancements, yet their training is resource-intensive and highly sensitive to hyper-parameter selection. While scaling laws provide valuable guidance on model size and data requirements, they fall short in choosing dynamic hyper-parameters, such as learning-rate (LR) schedules, that evolve during training. To bridge this gap, we present Optimization Hyper-parameter Laws (Opt-Laws), a framework that effectively captures the relationship between hyper-parameters and training outcomes, enabling the pre-selection of potential optimal schedules. Grounded in stochastic differential equations, Opt-Laws introduce novel mathematical interpretability and offer a robust theoretical foundation for some popular LR schedules. Our extensive validation across diverse model sizes and data scales demonstrates Opt-Laws' ability to accurately predict training loss and identify optimal LR schedule candidates in pre-training, continual training, and fine-tuning scenarios. This approach significantly reduces computational costs while enhancing overall model performance.

오 이건 굉장히 흥미로운 결과네요. DeepSeek 스타일의 하이퍼파라미터 Scaling Law와 (https://arxiv.org/abs/2401.02954) 최근의 Learning Rate Schedule에 대한 Scaling Law의 (https://arxiv.org/abs/2408.11029) 결합으로 생각해볼 수 있을 것 같습니다. 즉 작은 규모의 모델에 대한 실험을 통해 큰 모델의 LR, LR Schedule, Warmup Step 등을 결정할 수 있다는 것이죠.

MoE 모델을 타겟으로 실험했다는 것도 좋은 부분이네요.

#scaling-law #hyperparameter

# Links

[[240820 Scaling Law with Learning Rate Annealing.md]]
[[240105 DeepSeek LLM.md]]