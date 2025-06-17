https://openai.com/index/gpt-4o-mini-advancing-cost-efficient-intelligence/

GPT-4o mini가 등장하면서 이제 OpenAI, Google, Anthropic이 비슷한 성능과 비슷한 가격대에서 경쟁하게 됐다. 입력 $0.15/0.35/0.7, 출력 $0.6/0.7/1.25. Google이나 Anthropic도 다시 Flash, Haiku의 성능 개편 모델을 곧 내놓지 않을까 싶다.

사실 비용 자체보다는 이 비용으로도 충분한 가벼운 모델을 어떻게 만들었는지가 더 궁금하긴 하다. 한 가지 분명한 듯 싶은 것은 큰 모델을 만들고 그것을 기반으로 작은 모델을 만드는 것이 보편화 되어있다는 것. Gemini 1.5 Flash와 같이.

https://x.com/karpathy/status/1814038096218083497
https://www.youtube.com/watch?v=B45s_qWYUt8&t=752s

그런데 큰 모델을 어떻게 작은 모델로 압축하는가? 그 방법에서는 불확실한 부분이 많다. Knowledge Distillation 같은 기본적인 방법이라고 하더라도 어떤 데이터를 기반으로 Distill 할 것인지가 문제일 것이다. On-Policy Distillation 같은 방법의 변형도 생각해볼 수 있을 것 같고.

위에서 Karpathy와 Aidan Gomez가 언급하듯 합성 데이터가 중요한 부분일 것 같기는 한데 그 방법이 무엇인지는 알 수 없다. Karpathy는 웹 데이터의 문제가 지식과 사고가 얽혀 있다는 것이라고 말하고 Aidan Gomez는 자동화된 방식으로 모델의 약점을 찾아내고 그 부분에서 갭을 줄인다는 언급을 하는데 여전히 단서 수준이긴 하다.

추측하자면 웹 데이터에 대한 재작성, 자주 언급되어왔던 행간을 생성하는 것, 그리고 코드와 수학에 대한 자동화된 피드백을 통한 데이터 생성 정도가 큰 축이 아닐까 싶다. 물론 이 큰 방향 자체보다는 이 방법들을 작동하게 만들고 Scaling을 할 수 있게 만드는 트릭이 중요한 것이기는 하지만 말이다.