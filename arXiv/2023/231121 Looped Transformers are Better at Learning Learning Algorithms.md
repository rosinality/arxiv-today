https://arxiv.org/abs/2311.12424

Looped Transformers are Better at Learning Learning Algorithms (Liu Yang, Kangwook Lee, Robert Nowak, Dimitris Papailiopoulos)

In-context Learning에 대해 Mesa optimization이라는 아이디어에서 시작해 트랜스포머 자체를 SGD 같은 iterative algorithm을 더 잘 학습할 수 있도록 바꿔볼 수 있을까라는 아이디어네요. Universal Transformer나 Implicit Model과 비슷하게 하나의 레이어를 반복적으로 적용하되, 입력 임베딩을 매 반복마다 더해주는 차이가 있습니다. 추가로 학습 시에 레이어 적용 횟수의 최저값을 하이퍼파라미터로 지정하는 군요.

iteration의 증가에 따라 결과값이 고정점으로 수렴하는 모델이 되고, 학습 시 적용한 iteration보다 많은 iteration에 대해서도 일반화가 가능해지는 군요. 복잡도가 높은 함수에 대해서는 트랜스포머와 엇비슷한 것 같긴 합니다. 여하간 arbitrary depth 모델은 꽤 흥미로운 주제가 아닌가 싶습니다.

#in_context_learning #transformer 