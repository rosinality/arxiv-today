https://arxiv.org/abs/2311.16620

On the Long Range Abilities of Transformers (Itamar Zimerman, Lior Wolf)

Long Range Arena를 태클하는 연구는 오랜만에 보네요. Long Range Arena에서 트랜스포머가 약한 것은 표현력이나 최적화의 문제가 아니라 적절한 inductive bias의 부재에 따른 일반화 능력의 문제 때문이라는 이야기를 합니다.

그러면 성공적인 모델들에는 어떤 inductive bias가 있었는가를 보니 smooth하고 exponential decay가 들어간 conv kernel이 핵심이었다고 합니다. 그래서 attention에 exponential decay를 곱해주고 average pooling으로 smoothing을 추가했네요.

이 결과가 자연어에도 시사하는 바가 있을까요? 사실 자연어에서는 트랜스포머 보다 나은 특성을 보여준 사례가 없어서 적절한 inductive bias가 무엇인지를 논하는 것 자체가 어렵긴 합니다. 그래도 attention 패턴을 계속 들여다보면 LM-Infinite (https://arxiv.org/abs/2308.16137) 에서처럼 현재 attention의 중요한 문제를 발견할 수 있지 않을까 싶네요.

#long_context #transformer

# Links

