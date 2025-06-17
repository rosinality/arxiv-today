https://arxiv.org/abs/2312.16903

Spike No More: Stabilizing the Pre-training of Large Language Models (Sho Takase, Shun Kiyono, Sosuke Kobayashi, Jun Suzuki)

트랜스포머의 학습 불안정성을 Weight와 Embedding의 Scale을 줄이는 것으로 해결한다는 아이디어. Attention Score의 Normalizer sqrt(d)를 키우는 것으로 학습을 더 안정하게 할 수 있다는 트릭도 그렇고 출력의 크기가 학습에 꽤 영향을 미치는 것이 아닌가 싶네요.

Tero Karras가 하는 작업처럼 (https://arxiv.org/abs/2312.02696) 트랜스포머도 마음 먹고 튜닝하면 의외의 개선점들이 꽤 있을 수 있지 않을까 싶습니다.

#transformer #initialization #normalization

# Links

[[231205 Analyzing and Improving the Training Dynamics of Diffusion Models.md]]