https://arxiv.org/abs/2309.13638

Embers of Autoregression: Understanding Large Language Models Through the Problem They are Trained to Solve (R. Thomas McCoy, Shunyu Yao, Dan Friedman, Matthew Hardy, Thomas L. Griffiths)

Sparks of AGI (https://arxiv.org/abs/2303.12712) 를 겨냥한 제목이죠. LM이 굉장한 능력을 보여주고 있지만 Autoregressive Modeling으로 인해 발생하는 잔재가 있을 것이다...라는 생각입니다. 여러 가지가 있겠지만 주로 다루는 건 다음 세 가지네요.

1. 흔한 과제보다 드문 과제에 취약하다. 예를 들어 알파벳 순으로 정렬하는 것보다 역순으로 정렬하는 것에 약합니다.
2. 생성하는 텍스트의 확률이 낮은 경우 취약하다. 역순으로 나열된 단어를 정방향으로 뒤집는 과제를 시켜보면 정방향 텍스트가 더 확률이 높은 텍스트을 때 성능이 더 높습니다.
3. 입력 텍스트의 확률이 낮은 경우 취약하다. 다만 입력 텍스트에 대해서는 일반화가 더 잘 될 것이라고 예상했고, 실제로 효과가 크지 않네요.

사실 이런 것보다 논문에서 더 중요하게 말하고 싶은 건 (사람과 비슷한가를 보는 것이 아니라) LM을 LM이 학습한 목표와 과제의 측면에서 볼 필요가 있다는 메시지일 것 같네요. Thomas Griffith는 계산인지과학 쪽에서 유명한데 요즘 이런 작업도 하는군요.

#autoregressive_model #llm

# Links

[[230322 Sparks of Artificial General Intelligence.md]]