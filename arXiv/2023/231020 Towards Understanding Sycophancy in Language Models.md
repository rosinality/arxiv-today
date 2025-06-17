https://arxiv.org/abs/2310.13548

Towards Understanding Sycophancy in Language Models (Mrinank Sharma, Meg Tong, Tomasz Korbak, David Duvenaud, Amanda Askell, Samuel R. Bowman, Newton Cheng, Esin Durmus, Zac Hatfield-Dodds, Scott R. Johnston, Shauna Kravec, Timothy Maxwell, Sam McCandlish, Kamal Ndousse, Oliver Rausch, Nicholas Schiefer, Da Yan, Miranda Zhang, Ethan Perez)

정렬된 LLM의 아첨(Syncophancy)에 대한 분석. 여기서 아첨이란 유저의 입력에 응답이 영향을 받는 경우를 말하고, 텍스트에 피드백을 달라고 했을 때 유저의 텍스트에 대한 평가에 좌우된다거나, QA 상황에서 유저의 판단이나 믿음에 따라 답이 달라진다거나, 유저의 실수를 따라한다거나 하는 현상입니다.

이런 현상이 발생하는 이유는? 일단 RLHF 데이터셋에 유저의 믿음과 일치하는 경우 선호되는 경향이 강하게 있군요. 그런데 Preference Model과 RLHF 상황으로 가면 문제가 좀 복잡해집니다. BoN에서는 피드백 상황을 제외하면 아첨이 억제되는 경향이 나타났습니다. 프롬프팅으로 아첨을 억제하면 대체로 더 억제되는 경향이 나타나네요. 그런데 RLHF로 가면 피드백과 실수 모방에서 아첨이 늘어나는 경향이 발생합니다.

그래서 Preference Model을 좀 더 분석합니다. 여기서 중요하게 보는 것은 난이도(오해하기 쉬운 정도)에 따른 패턴 변화에 대한 관찰이네요. 사람에 대해서도 데이터를 수집해서 관찰했는데, 사람과 모델 모두 난이도가 높아질수록 유저의 믿음에 동조하는 응답을 선호하는 패턴이 발생하네요.

결과를 종합적으로 정리하기가 좀 어렵다고 느껴지는데...제 생각에 따라 정리해보면 다음과 같습니다.

1. 강력한 Preference Model은 아첨을 억제할 수도 있다. 그렇지만 특정 부문에서는 억제하는 것이 아니라 촉진하는 경향도 나타난다. 그러나 아첨을 억제하는 경우에도 인위적으로 아첨을 억제한 Preference Model에 비해서는 아첨을 충분하게 억제하지 못한다.
2. BoN에 비해 RLHF에서 아첨 억제 경향이 약하다. Preference Model의 아첨 선호 특성을 RLHF가 해킹하고 있을 수 있다는 증거로 보인다.
3. 질문의 난이도가 높아질수록, 즉 전문성이 필요한 질문으로 나아갈수록 사람을 통한 데이터 수집 과정에서 아첨을 억제하기가 어렵다. 정확히는 그 문제에 대한 전문성이 없는 사람이 정확한 답을 선호하기가 어렵다.

사실 가장 중요한 포인트는 비전문가의 피드백을 사용하는 것을 넘어서는 방법이 필요하다는 것일 것 같네요. (물론 전문가의 피드백을 적극적으로 반영하는 것도 가능한 방법이겠죠.) 그 방법이 무엇일지에 대해서는 직접 언급하지 않지만, 인용하고 있는 논문들은 AI를 적절하게 결합하는 방법에 타개책이 있을 수 있지 않은가를 시사하고 있군요. (https://arxiv.org/abs/1811.07871, https://arxiv.org/abs/1805.00899, https://arxiv.org/abs/2212.08073, https://arxiv.org/abs/2211.03540)

근본적으로는 RL로 사람을 뛰어넘는 수준의 퍼포먼스에 도달할 수 있다. 그런데 사람을 뛰어넘을 수 있게 해줄 Reward는 어떻게 만들 수 있을 것인가? 라는 문제로군요. 지금은 비전문가의 수준을 뛰어넘는 Reward를 만드는 단계인 것이고요.

#alignment #rl

# Links

[[230221 Anthropic.md]]