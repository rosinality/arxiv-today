https://arxiv.org/abs/2311.01462

Idempotent Generative Network (Assaf Shocher, Amil Dravid, Yossi Gandelsman, Inbar Mosseri, Michael Rubinstein, Alexei A. Efros)

idempotent function, f(f(x)) = f(x) 으로 생성 모델을 구성. 이미지 x에 대해 f(x) = x를 학습, 노이즈 z에 대해 f(f(z)) = f(z)를 학습. f(z) = z라는 trivial한 결과로 이어지는 것을 막기 위해 f'(f(z)) != f(z)를 학습. 생성 모델의 기본적인 문제인 노이즈와 이미지 사이의 매핑을 어떻게 정의할 것인가? 에 대한 새로운 접근이라고 할 수 있지 않을까 싶네요. 얼핏 보면 GAN과도 연결지을 수 있는 부분이 있지 않을까 싶습니다.

이런 형태를 사용해서 가능한 것이라고 하면 특별한 학습 없이도 노이지한 이미지, 흑백이나 스케치 입력에 대해서도 이미지 생성이 된다느 것이네요. trivial한 결과로 이어지는 것을 강제로 막는 형태라 까다로울 것 같긴 합니다만 재미있네요.

#generative_model 