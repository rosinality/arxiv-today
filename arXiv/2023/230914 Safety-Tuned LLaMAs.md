https://arxiv.org/abs/2309.07875

Safety-Tuned LLaMAs: Lessons From Improving the Safety of Large Language Models that Follow Instructions (Federico Bianchi, Mirac Suzgun, Giuseppe Attanasio, Paul Röttger, Dan Jurafsky, Tatsunori Hashimoto, James Zou)

safety 데이터를 만들어서 sft를 해봤군요. 발견한 것은 1. safety 데이터가 조금 추가되면 harmful response가 크게 감소한다. 2. safety 데이터를 너무 많이 쓰면 과장된 safe response가 발생한다. 3. 모델이 unsafe한 문제에 대한 의견을 구하는 형태의 instruction에 대해 안전한 의견을 낸다고 하더라도, 실제로 그 unsafe한 질문을 했을 때 안전한 응답을 한다는 것은 아니다. 어제 나온 SafetyBench (https://arxiv.org/abs/2309.07045) 같은 형태의 벤치마크를 고려할 때 주의해야할 부분이겠죠.

#safety #alignment

# Links

[[230913 SafetyBench.md]]