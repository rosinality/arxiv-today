https://arxiv.org/abs/2309.15505

Finite Scalar Quantization: VQ-VAE Made Simple (Fabian Mentzer, David Minnen, Eirikur Agustsson, Michael Tschannen)

Vector Quantization의 대안. 스칼라를 정수로 반올림하고 straight through estimator를 사용했습니다. 정수 변환을 통해 가능한 값을 L개로 맞추는데, 차원을 늘리면 코드북의 크기를 큰 문제 없이 확장할 수 있네요.

성능은 대략 VQ와 비슷하게 나옵니다만 좀 더 심플하고, 특별한 트릭 없이 코드북 크기를 키워도 코드북 활용률 100%를 달성할 수 있다는 것이 장점이군요.

#vq 
