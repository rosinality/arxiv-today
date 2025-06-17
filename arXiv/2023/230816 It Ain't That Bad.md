https://arxiv.org/abs/2308.08268

It Ain't That Bad: Understanding the Mysterious Performance Drop in OOD Generalization for Generative Transformer Models (Xingcheng Xu, Zihao Pan, Haipeng Zhang, Yanqing Yang)

사칙연산이 트랜스포머의 ood generalization의 한계를 보여주는 예제로 흔히 사용되는데...여기서는 ood 상황에서 트랜스포머 응답의 패턴을 봤습니다. 흥미로운 것은 3 자리 숫자의 덧셈이나 곱셈으로 학습시켰을 때 4 자리 숫자 (ood)를 입력하면 천의 자리 숫자를 무시한다는 결과를 얻었네요.

즉 a + b에 대해서 (a mod 10^3) + (b mod 10^3) 이 결과로 나온다는 것입니다.

물론 이렇게 천의 자리 숫자를 무시하고 나머지 3 자리에 대해서 작동하는 패턴이 보인다고 해도 이걸 어떻게 잘 뜯어고치면 4 자리 숫자에 대해서도 일반화 되도록 동작하게 만들 수 있다는 의미가 되는 것은 아니지만...흥미로운 사실인 것 같네요.

#transformer #generalization 