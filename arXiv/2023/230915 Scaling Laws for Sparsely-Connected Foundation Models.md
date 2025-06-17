https://arxiv.org/abs/2309.08520

Scaling Laws for Sparsely-Connected Foundation Models (Elias Frantar, Carlos Riquelme, Neil Houlsby, Dan Alistarh, Utku Evci)

weight sparse 모델에 대한 scaling law. optimal sparsity contour이 핵심적이라고 할 수 있을 듯 한데, pretraining flops와 non zero parameter의 수에 대해 최저 loss를 달성하는 sparsity 수준에 대한 커브입니다. Chinchilla (dense optimal 모델) 보다 더 많은  pretraining flops를 투입할 수록 optimal sparsity의 수준 또한 올라간다는 것이 메인 포인트군요.

또한 같은 flops를 투입했을 때 sparse 모델이 (파라미터 수로 따졌을 때) 몇 배의 파라미터를 가진 dense 모델과 동일할 것인가를 추산하는 것도 가능합니다.

sparse 모델을 효율적으로 학습과 추론에 쓸 수 있다고 한다면 weight sparsity가 유용한 도구가 될 수 있다는 것을 시사하는 것으로 보이네요. moe와 비교하면 어떨까도 흥미로운 부분이겠습니다.

#sparsity #efficient_training #efficiency 