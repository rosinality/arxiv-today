https://arxiv.org/abs/2309.17453

Efficient Streaming Language Models with Attention Sinks (Guangxuan Xiao, Yuandong Tian, Beidi Chen, Song Han, Mike Lewis)

LM으로 생성을 쭉 이어나가다가 context length를 넘어버리는 상황이 되면 어떻게 대응할 것인가. window attention 느낌으로 key-value cache를 자른 다음 생성을 이어나가는 방식으로 할 수 있다면 좋겠지만 그러면 작동을 하지 않는다고 하죠. 왜? 첫 부분의 토큰이 중요하기 때문이라고 합니다.

그렇다면 첫 부분의 토큰이 중요한 이유는? 초기 토큰을 attention sink로 쓰기 때문이라고 합니다. softmax에서는 전체가 0이 될 수 없는데 트랜스포머에서는 전체가 0인 attention이 필요한 경우가 있고, 그래서 특정 토큰을 사용해 그 역할을 하도록 한다는 것입니다. 그게 왜 하필 초기 토큰인가 하면 아무래도 초기 토큰은 모든 토큰에서 접근이 가능하니 그 방향으로 학습이 되는 경향이 있을 수 있겠네요.

이 문제는 비교적 최근 발견되었고 (https://arxiv.org/abs/2306.12929) 거기에 대해 softmax의 분모에 1을 더해놓으면 어떨까 (https://www.evanmiller.org/attention-is-off-by-one.html) 하는 대응 방법도 논의된 적이 있습니다.

여하간 첫 부분의 토큰이 문제이니 첫 부분의 토큰 임베딩 캐시를 유지하면 문제가 없다는 발견입니다. window attention과 결합하면 제목 그대로 context length를 넘는 경우에도 streaming generation이 가능해지는 것이죠.

더 나아가 학습 시점부터 attention sink를 도와주는 방식으로 할 수는 없을까 하는 실험도 했습니다. zero key-value를 사용해 위의 softmax off by one을 테스트해봤는데 이 방법만으로는 충분하지 않은 것으로 보입니다. learnable token을 사용하면 잘 작동하는 것으로 보이네요.

초기 토큰이 중요하다는 것은 context length 연장이라는 측면에서도 논의된 적이 있습니다. (https://arxiv.org/abs/2308.16137) 트랜스포머의 특성에 대한 꽤 중요한 발견이 될 것 같네요.

#lm #efficiency #transformer

# Links

[[230622 Quantizable Transformers.md]]
[[230830 LM-Infinite.md]]