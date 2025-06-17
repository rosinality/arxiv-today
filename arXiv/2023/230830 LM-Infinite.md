https://arxiv.org/abs/2308.16137

LM-Infinite: Simple On-the-Fly Length Generalization for Large Language Models (Chi Han, Qifan Wang, Wenhan Xiong, Yu Chen, Heng Ji, Sinong Wang)

context length 뻘글을 쓰자마자 또...우선 lm에서 ood length generalization이 안 되는 이유를 분석.

1. 학습에서 보지 않은 거리의 토큰들을 보게 되어서. relative pe의 경우 학습에 보지 않은 거리에 있는 토큰들에 대해 logit이 증가하는데 이것이 모델에서 다시 ood 값이 될 수 있음.

2. 또한 logit이 증가하지 않는 이상 입력 토큰 수가 많아질수록 attention의 entropy가 증가함.

3. 그렇다면 attention window를 제한하면 되지 않을까? 그렇지만 lm은 positional embedding이 없는 상황에도 위치 정보가 인코딩 되어 있기 때문에 초기 토큰과 이후 토큰을 구분하는 경향이 있고, window를 만들어 초기 토큰이 사라져버리면 다시 ood 상황이 발생하게 됨.

그래서 제안하는 방법. 놀랍게도 BigBird (https://arxiv.org/abs/2007.14062) 같은 global attention + local attention의 조합. 프리트레이닝에서 봤던 context length를 window로 해서 local attention을 잡고, 추가적으로 앞 부분 토큰 N개를 볼 수 있도록 global attention을 설정.

결과적으로 perplexity, generation, key retrieval에서 일정 정도 결과를 보여줌. positional embedding의 특성이나 프리트레이닝 시점의 local attention의 가능성에 대해서 생각해볼 필요가 있을까 싶기도.

#transformer

# Links

[[200727 Big Bird.md]]