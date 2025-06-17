https://arxiv.org/abs/2310.04373

Confronting Reward Model Overoptimization with Constrained RLHF (Ted Moskovitz, Aaditya K. Singh, DJ Strouse, Tuomas Sandholm, Ruslan Salakhutdinov, Anca D. Dragan, Stephen McAleer)

이 논문은 우선 (제목에도 나와 있지만) Reward Model Overoptimization 문제에 대한 태클이다. 이건 Reward 모델에서 나오는 Reward 스코어는 향상됐는데 실제 성능은 떨어지는 상황을 말한다. 예를 들어 자세하게 설명하는 걸 Reward 모델이 선호하다 보니 장황한 텍스트를 생성한다거나 하는 상황이다. 추가적으로 Reward 모델이 두 개 이상 있는 경우를 생각한다.

아이디어는 이렇다. Reward 스코어가 일정 지점(역치)를 넘어서면 성능이 떨어지는 현상이 일어난다고 하자. 각 Reward 모델에 대해 이런 역치를 찾을 수 있다면, 이 역치를 넘지 않도록 제약 조건을 걸고 PPO를 하자는 것이다. 제약 조건 하의 최적화 문제는 라그랑주 승수로 풀고.

흥미롭지만 두 개 이상의 Reward 모델을 쓰는 상황이 (충분히 있을 수 있지만) 바로 많이 생각나지는 않고, 또 역치는 어떻게 찾아야 할 것인가 하는 생각도 든다. 물론 논문에서 역치를 좀 더 효율적으로 찾을 수 있는 방법에 대해서도 논하기는 한다.

https://arxiv.org/abs/2310.12773

Safe RLHF: Safe Reinforcement Learning from Human Feedback (Josef Dai, Xuehai Pan, Ruiyang Sun, Jiaming Ji, Xinbo Xu, Mickel Liu, Yizhou Wang, Yaodong Yang)

그런데 RLHF 상황에서 Reward 모델을 두 개 쓰는 대표적인 상황이 하나 있다. Helpfulness와 Harmlessness Reward 모델을 분리하는 경우. Llama 2 (https://arxiv.org/abs/2307.09288) 에서는 이 두 모델을 프롬프트나 샘플이 안전 기준을 넘는 상황에서 Harmlessness Reward 모델을 사용하는 방식으로 결합했다.

Safe RLHF에서는 이를 Harmlessness 모델인 Cost 모델 C와 Helpfulness 모델인 Reward 모델 R을 다음과 같은 방식으로 결합하는 방식으로 접근했다.

max R(y, x) such that C(y, x) <= 0

그러니까 Harmlessness 제약 조건 하에서 Helpfulness를 최대화하는 문제가 된다. 위의 제약 조건 하의 RLHF와 같은 상황이라 할 수 있고, 마찬가지로 라그랑주 승수를 적용해 대응했다.

Helpfulness와 Harmlessness에 대한 꽤 좋은 결합 방식으로 보이고, 이 결과를 보고 나니 제약 조건 하에서 Reward 스코어를 최적화하는 것이 의미있을 수 있는 사례가 충분히 더 있겠다는 생각이 든다. 예를 들어 진실성 제약 조건을 건 상태에서 창조성을 최대화한다든가, 혹은 퀄리티 제약 조건을 건 상태에서 다양성을 최대화한다거나. 지금이야 각각도 태클하기 어려운 문제이긴 하지만 곧 종합적으로 접근하는 것이 필요해지지 않을까 싶다.

https://arxiv.org/abs/2310.10638

In-Context Pretraining: Language Modeling Beyond Document Boundaries (Weijia Shi, Sewon Min, Maria Lomeli, Chunting Zhou, Margaret Li, Victoria Lin, Noah A. Smith, Luke Zettlemoyer, Scott Yih, Mike Lewis)

지금 LM 프리트레이닝에서는 랜덤한 문서들을 가져다 붙여 특정 길이(2K, 4K 등)로 만든 다음 학습시키는 방식을 쓴다. 그러니까 기본적으로는 서로 상관 없는 텍스트들이 연결되어 있는 것이다. 그래도 잘 돌아가긴 하지만, 문제를 찾아본다면 우선 텍스트들이 서로 관계가 없으니 그 내부에서 유의미한 정보 교환이 일어나지 않을 것이고, 그러니 학습시에 입력되는 길이의 텍스트를 충분히 활용하도록 학습하기가 좀 어려울 것이다. 거기다 유의미한 정보 교환이 없는 텍스트들 사이에 Attention을 계산한다는 것 자체가 비효율적이라고 볼 수 있다.

그렇다면 서로 관계 있는 텍스트들을 붙여서 학습 데이터를 구성하면 어떨까? 그런데 그러려면 엄청난 규모의 프리트레이닝 코퍼스를 유사도 순으로 정렬하는 문제를 풀어야 한다. (각 텍스트에서 가장 유사한 텍스트를 인출해오는 식으로 하면 특정 텍스트를 여러 번 보게 될 수 있으니 한계가 있다. 즉 텍스트를 한 번만 보면서도 서로 유사한 텍스트가 인접하도록 정렬하는 문제가 된다.) 논문에서 제안하는 것은 이 정렬 문제를 효율적으로 푸는 방법이다.

어떻게 보면 Retrieval 기반 프리트레이닝을 (https://arxiv.org/abs/2310.07713, https://arxiv.org/abs/2310.07713) 인코더 대신 디코더 only 구조에서 앞쪽 컨텍스트에 붙여주는 방식으로 접근한 것과 비슷하다고 할 수도 있을 듯 하다. 그렇다면 Retrieval 기반 모델의 장점을 어느 정도 가져올 수 있지 않을까.

대규모 코퍼스에 대해 정렬 문제를 풀어야 한다는 것 자체가 부담이긴 하지만 이 방법이 어떤 의도하지 않은 문제를 발생시킬만한 부분은 그다지 없지 않을까 싶다. 한 가지 생각해보자면 컨텍스트를 활용하는 방식으로 학습되었기에 컨텍스트가 주어지지 않는 상황이 약점이 될 수 있지 않을까. 컨텍스트가 없는 상황에서 응답하려면 지식을 많이 습득하는 게 필요할 텐데 그런 경향은 약화될 수 있지 않을까 싶다. 혹은 늘 문제가 되는 규모가 커지니 향상이 감소할 수 있는 가능성도 있긴 하다. 그 위험을 제외하면 프리트레이닝에 대한 유의미한 개선이 될 수 있지 않을까?

서로 관계 있는 텍스트들을 인접하게 배치한다는 것은 RNN으로 LM을 하던 시절에 중요한 트릭이었다. 물론 거기서는 하나의 텍스트가 배치 간에 이어지게 만든 것이고, 여기서는 한 컨텍스트 내에 인접하도록 만드는 것이긴 하지만 기능적으로는 좀 비슷하다고 할 수 있지 않을까 싶다.

https://openreview.net/forum?id=AL1fq05o7H

Mamba: Linear-Time Sequence Modeling with Selective State Spaces

사실 트랜스포머가 모든 것을 점령하고 있는 지금 시점에 오히려 RNN, State Space Model에서 더 흥미로운 탐색들이 더 많이 보이고 있는 것 같기도 하다. Mamba의 핵심은 State Space Model의 각 파라미터들이 입력에 따라 변화할 수 있도록 만든 것이다.

요즘 이런 모델들에 요청되는 것들이 많아서 그런지 실험도 많고 가속을 위한 커널도 만들었다. 트랜스포머와의 비교도 바닐라 트랜스포머로는 재미가 없으니 RoPE와 SwiGLU 등을 붙인 최신 유행 버전 트랜스포머 베이스라인도 같이 나와 있고. 물론 그렇다고 하더라도 더 큰 규모에서 하면 어떤가 하는 질문은 나올 수밖에 없다.

RNN 시절에는 텍스트 전체의 정보를 고정 크기 벡터로 압축할 수 없다는 한계가 중요한 문제였다면, 지금은 워낙 레이어도 많고 차원도 크기 때문에 그 주장으로 일관하는 것은 그리 적절하지 않은 것 같다. 지금 규모에서는 집어넣는다면 집어넣을 수 있을 것 같기 때문에...거기에 요즘 모델들은 상태가 모델 차원의 K배 크기의 행렬이기 때문에 더 여유가 있다.

그래서 결과적으로 트랜스포머와 비슷한 수준의 벤치마크 수치를 찍을 수 있다면 RNN 특유의 추론 시점의 효율성이 큰 장점이 될 것이고, 또 RNN의 Inductive Bias가 유의미한 도움이 될 수도 있겠다. 물론 이것은 더 큰 규모에서 트랜스포머 수준의 결과를 달성할 수 있다는 것이 확인된 이후의 이야기이긴 하다.

예전이라면 어렵지 않을까 싶었는데 곧 의미 있는 결과가 나올 수 있지 않을까 싶다.

https://cdn.openai.com/papers/dall-e-3.pdf

Improving Image Generation with Better Captions (James Betker, Gabriel Goh, Li Jing, Tim Brooks, Jianfeng Wang, Linjie Li, Long Ouyang, Juntang Zhuang, Joyce Lee, Yufei Guo, Wesam Manassra, Prafulla Dhariwal, Casey Chu, Yunxin Jiao, Aditya Ramesh)

DALLE-E 3에 대한 테크니컬 리포트. 요즘 방법조차 말하지 않는 리포트보다는 좀 나아서 대략 어떻게 했다 정도의 이야기는 하고 있다. 역시나 이미지-텍스트 페어에 대해 캡션을 새로 생성한 것이 메인이다. 거기에 GPT-4로 프롬프팅을 해서 사용자 입력을 상세한 이미지 생성 프롬프트로 바꾸는 방법에 대한 언급도 하고 있다.

이미지-텍스트 페어 데이터를 사용한 멀티 모달 모델에 큰 발전이 있었지만...대규모로 용이하게 구할 수 있는 이미지-텍스트 데이터의 품질이 그다지 좋지 않다는 것이 아쉬운 부분이지 않았나 싶다. 그런 의미에서 한 가지 할 수 있는 부분이 이런 식의 캡셔닝을 통한 텍스트 개선일 것이다. (https://arxiv.org/abs/2310.00426) 다른 방법으로는 이미지나 텍스트 유니 모달 데이터를 사용해 각 유니 모달에 대한 표현 능력을 향상시키는 것이 있지 않은가 싶다. (https://arxiv.org/abs/2310.08825) 그리고 이를 종합적으로 연결하는 방법도 있을 수 있겠다. (https://arxiv.org/abs/2310.03734)