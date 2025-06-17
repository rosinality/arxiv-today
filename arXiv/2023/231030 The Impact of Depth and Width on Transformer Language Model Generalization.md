https://arxiv.org/abs/2310.19956

The Impact of Depth and Width on Transformer Language Model Generalization (Jackson Petty, Sjoerd van Steenkiste, Ishita Dasgupta, Fei Sha, Dan Garrette, Tal Linzen)

트랜스포머의 넓이 vs 깊이. 여기서는 좀 특이하게 모델(임베딩) 차원은 고정하고 ffn의 hidden dimension과 레이어의 수를 바꿔가면서 테스트해봤네요. 뉴럴넷 판의 교훈처럼 넓은 모델보다 깊은 모델이 낫다, 그렇지만 깊이 상승에 따라 성능 향상폭은 감소하고 ffn hidden dimension이 임베딩 차원 이하로 가는 순간 성능이 감소하기 시작한다는 것이 나타나네요.

compositional generalization에서 깊이의 역할에 대해서도 논하고 있습니다만 사실 결과로 봐선 compositional generalization에서도 쉬운 것만 풀리는 것이 아닌가 하는 느낌이네요.

조금 다른 이야기지만 트랜스포머의 레이어 수는 동작하는 알고리즘의 복잡도나 단계를 결정한다는 느낌이 있고, 그런 의미에서 Universal Transformer나 Equilibrium Model 같은 임의 깊이 모델들에서도 뭔가 다음 세대 모델에 대한 힌트를 발견할 수 있지 않을까? 하는 생각이 드네요.

#transformer 