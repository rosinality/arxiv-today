https://cdn.openai.com/papers/weak-to-strong-generalization.pdf

Weak-to-Strong Generalization: Eliciting Strong Capabilities With Weak Supervision (Collin Burns, Pavel Izmailov, Jan Hendrik Kirchner, Bowen Baker, Leo Gao, Leopold Aschenbrenner, Yining Chen, Adrien Ecoffet, Manas Joglekar, Jan Leike, Ilya Sutskever, Jeff Yu)

약한 모델이 생성한 데이터로 강한 모델을 튜닝했을 때의 성능을 얼마나 개선할 수 있는가? 하는 문제입니다. 의도는 사람이 사람을 뛰어넘는(Superhuman) 수준의 모델을 어떻게 튜닝할 수 있는가 하는 것이죠. Anthropic에서도 비슷한 연구를 했었죠. (https://arxiv.org/abs/2211.03540)

일단 약한 모델이 생성한 데이터로 학습했을 때 강한 모델이 약한 모델보다 나은 성능을 보여주는 현상은 나타납니다. 성능을 더 개선하기 위해서 모델 크기 순서대로 레이블을 만들고 튜닝하는 것과 (Bootstrapping) 강한 모델 자체의 Confidence를 사용해 Pseudo Label을 만들어 Regularization 하는 방법을 테스트해봤습니다. 레이블과는 별개로 데이터 자체에 대해 Autoregressive 학습을 시키는 방법도 테스트해봤군요.

아직 갭이 있지만 점진적으로 갭을 줄여나갈 수 있는 가능성은 확인된 것 같네요. Weak Supervision 같은 고전적인 문제가 이 맥락에서 다시 등장했다는 것이 흥미롭습니다.

#alignment 