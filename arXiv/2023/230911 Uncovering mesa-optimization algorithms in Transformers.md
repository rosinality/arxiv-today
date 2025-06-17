https://arxiv.org/abs/2309.05858

Uncovering mesa-optimization algorithms in Transformers (Johannes von Oswald, Eyvind Niklasson, Maximilian Schlegel, Seijin Kobayashi, Nicolas Zucchet, Nino Scherrer, Nolan Miller, Mark Sandler, Blaise Agüera y Arcas, Max Vladymyrov, Razvan Pascanu, João Sacramento)

transformer 내부에서 gradient descent가 발생할 수 있고 또 그렇다는 아이디어가 있었죠. (https://arxiv.org/abs/2212.07677) 이 논문에서는 in context learning 상황이 아니라 autoregressive 상황에서 이러한 최적화(mesa optimization)이 발생할 수 있는지를 분석합니다.

그런데 이게 좀 까다로운 게 causal mask가 있을 때는 online gradient descent가 발생해서 최적이 아니라는 연구가 얼마 전에 나왔었죠. (https://arxiv.org/abs/2308.06912) 그래서 여기서는 대안적인 알고리즘을 고안한 다음 이 알고리즘이 transformer 내부에서 나타날 수 있는지를 관찰했습니다. 거기에 이 mesa optimization 자체를 수행하는 레이어를 디자인하기도 했네요.

synthetic한 세팅에서 실험한 결과에서 제안된 알고리즘을 probing으로 확인했고, 이 synthetic한 모델이 synthetic한 few shot 과제에서 in context learning을 할 수 있다는 것을 발견했네요. 덤으로 induction head도 재발견했습니다. (https://arxiv.org/abs/2209.11895)

자연어에 대해서도 실험해봤는데 분명하진 않지만 이런 optimization이 자연어 autoregressive 모델에서도 발생하고 있지 않을까? 하는 추측을 하고 있네요. 굉장히 흥미롭습니다.

#transformer #in_context_learning #autoregressive_model

# Links

[[230814 CausalLM is not optimal for in-context learning.md]]
[[220924 In-context Learning and Induction Heads.md]]