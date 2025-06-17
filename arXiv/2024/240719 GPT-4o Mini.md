https://openai.com/index/gpt-4o-mini-advancing-cost-efficient-intelligence/

*GPT-4o mini: advancing cost-efficient intelligence* (OpenAI)

GPT-4o mini가 나왔습니다. Gemini 1.5 Flash와 Claude Haiku보다 더 고성능이면서 더 저렴하다고 합니다. (1M 입력에 $0.15, 출력에 $0.6)

https://x.com/karpathy/status/1814038096218083497

사실 성능이나 가격보다 더 궁금한 건 이런 경량 모델들은 대체 어떤 방법으로 만들어지고 있는가겠죠. 일단 큰 모델을 만들고 그 모델을 사용해 작은 모델을 만든다는 흐름이 맞는 것 같은데 큰 모델을 어떻게 활용하는가 부분에는 밝혀지지 않는 것이 많네요. Knowledge Distillation 같은 기본적인 방법 이상으로 합성 데이터를 적극적으로 사용하고 있을 것 같긴 합니다.

Karpathy의 표현에 따르면 웹 데이터에 대한 프리트레이닝 어려운 이유는 지식과 사고가 서로 얽혀 있기 때문이라는 것입니다. 따라서 이 둘을 분리하는 것이 합성 데이터의 역할이라는 의미일 듯 한데 어쩌면 행간을 생성하는 것이 한 부분일지도 모르겠다 싶네요.

#llm #synthetic-data 