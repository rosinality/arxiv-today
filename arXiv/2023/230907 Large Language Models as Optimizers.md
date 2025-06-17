https://arxiv.org/abs/2309.03409

Large Language Models as Optimizers (Chengrun Yang, Xuezhi Wang, Yifeng Lu, Hanxiao Liu, Quoc V. Le, Denny Zhou, Xinyun Chen)

blackbox optimization을 llm으로 풀기. 기본적으로 이전에 파라미터 x에 대해서 나온 결과들을 주고 다음 파라미터를 찍어보라고 프롬프팅을 합니다. traveling salesman problem 같은 걸 풀어보는데, 놀랍게도 되긴 하지만 효율적이진 않죠.

그래서 좀 더 흥미로운 응용인 프롬프트 최적화를 테스트해봤네요. 결과가 꽤 재미있습니다. GSM8K에서 Let’s think step by step을 Take a deep breath and work on this problem step-by-step로 개선했군요.

#llm #optimization 