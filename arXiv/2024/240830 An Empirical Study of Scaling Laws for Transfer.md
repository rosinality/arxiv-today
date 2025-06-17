https://arxiv.org/abs/2408.16947

*An Empirical Study of Scaling Laws for Transfer* (Matthew Barnett)

> We present a limited empirical study of scaling laws for transfer learning in transformer models. More specifically, we examine a scaling law that incorporates a "transfer gap" term, indicating the effectiveness of pre-training on one distribution when optimizing for downstream performance on another distribution. When the transfer gap is low, pre-training is a cost-effective strategy for improving downstream performance. Conversely, when the gap is high, collecting high-quality fine-tuning data becomes relatively more cost effective. Fitting the scaling law to experiments from diverse datasets reveals significant variations in the transfer gap across distributions. In theory, the scaling law can inform optimal data allocation strategies and highlights how the scarcity of downstream data can bottleneck performance. Our findings contribute to a principled way to measure transfer learning efficiency and understand how data availability affects capabilities.

프리트레이닝-파인튜닝 시나리오에서의 Scaling Law. 프리트레이닝과 파인튜닝 데이터에 대한 Power Law, Irreducible Loss, 그리고 프리트레이닝-파인튜닝의 갭으로 구성된 형태입니다.

이런 식으로 생각해볼 수 있을 듯 하네요. 프리트레이닝-파인튜닝의 갭이 존재한다면 프리트레이닝에 아무리 많은 데이터를 사용하더라도 파인튜닝 성능을 개선하는데 상한이 있다는 것이고 추가적인 성능을 얻기 위해서는 파인튜닝 데이터가 필요하다는 것이죠.

물론 논문에서도 지적하는 것처럼 모델 크기에 대한 요소가 고려되어 있지 않긴 합니다. 모델이 커지면 이 갭이 함께 감소할 가능성이 높겠죠.

#scaling-law 