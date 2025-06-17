https://arxiv.org/abs/2309.02411

Delta-LoRA: Fine-Tuning High-Rank Parameters with the Delta of Low-Rank Matrices (Bojia Zi, Xianbiao Qi, Lingzhi Wang, Jianan Wang, Kam-Fai Wong, Lei Zhang)

ReLoRA와 [[230711 Stack More Layers Differently]] 비슷한 아이디어라는 느낌이군요. optimizer state와 lr을 조정하는 대신 업데이트된 lora weight와 이전 lora weight의 차이를 메인 파라미터에 반영하는 방식입니다. 이런 식의 low rank adaptation을 사용해 full rank training으로 전환하는 방법이 꽤 흥미롭다고 생각하는데...더 좋은 결과들이 나올지 궁금하네요. low rank gradient approximation과 대략 비슷한 걸까요?

#efficiency #efficient_training 