https://arxiv.org/abs/2406.12907

*Reconciling Kaplan and Chinchilla Scaling Laws* (Tim Pearce, Jinyeop Song)

> Kaplan et al. [2020] ('Kaplan') and Hoffmann et al. [2022] ('Chinchilla') studied the scaling behavior of transformers trained on next-token language prediction. These studies produced different estimates for how the number of parameters ($N$) and training tokens ($D$) should be set to achieve the lowest possible loss for a given compute budget ($C$). Kaplan: $N_\text{optimal} \propto C^{0.73}$, Chinchilla: $N_\text{optimal} \propto C^{0.50}$. This note finds that much of this discrepancy can be attributed to Kaplan counting non-embedding rather than total parameters, combined with their analysis being performed at small scale. Simulating the Chinchilla study under these conditions produces biased scaling coefficients close to Kaplan's. Hence, this note reaffirms Chinchilla's scaling coefficients, by explaining the cause of Kaplan's original overestimation.

Kaplan Scaling Law의 Model Scaling은 C^0.73으로 Chinchilla Scaling의 C^0.5와는 큰 차이가 있죠. 이 차이의 원인을 최적화 전략의 차이나 데이터셋의 차이로 생각했었는데, Kaplan Scaling Law에서 파라미터 수에서 임베딩을 빼고 생각했다는 것이 작은 규모에서 실험한 것과 맞물려 차이를 만든 것이라는 설명입니다.

차이를 발견하자면 얼마든지 발견할 수 있을 텐데 결과적으로 비슷한 Scaling Law로 귀결된다는 것이 놀랍네요.

#scaling-law 