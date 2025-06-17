https://arxiv.org/abs/2308.07037

Bayesian Flow Networks (Alex Graves, Rupesh Kumar Srivastava, Timothy Atkinson, Faustino Gomez)

Alex Graves는 요즘 어떤 작업을 하고 있는지 궁금했는데 이런 걸 하고 있었군요. (NNAISENSE라는 회사를 타이틀로 달고 있네요.)

diffusion 모델과 비슷한데 노이즈가 추가된 샘플 위에서 작동하는 diffusion 모델과는 달리 데이터 분포에 대한 파라미터를 업데이트하는 방식으로 작동하는 모델입니다.

베이지안 모델이 늘 그렇듯 흥미롭긴 합니다. 다만 어떤 강점이 있는지가 그냥은 명확하게 보이진 않네요. 일단 텍스트 시퀀스 같은 discrete 데이터에 대해 미분 가능한 방식으로 접근할 수 있다는 것이 한 가지 포인트인 듯 합니다.

#ddpm 