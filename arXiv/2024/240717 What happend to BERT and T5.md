https://www.yitay.net/blog/model-architecture-blogpost-encoders-prefixlm-denoising

*What happened to BERT & T5? On Transformer Encoders, PrefixLM and Denoising Objectives* (Yi Tay)

Yi Tay의 인코더와 Denoising에 대한 이야기. 인코더-디코더, 디코더, PrefixLM이 서로 그렇게 다른 것이 아니고 Denoising이나 Autoregressive LM은 어떤 구조에나 적용할 수 있다는 이야기, 모델이 커지면 이런 아키텍처의 차이는 크게 중요하지 않을 수 있다는 것, Denoising Objective를 사용하면 한 시퀀스에서 학습에 사용되는 토큰의 비율이 낮다는 것이 문제라는 통상적인 이야기를 합니다.

사실 가장 흥미로운 것은 Deonising Objective가 Autoregressive LM과 결합되었을 때 어떤 효과를 가질 것인가인데 장점이 있을 수 있다고 하긴 하지만 명확하게 이야기는 하지 않습니다. Yi Tay 본인은 무언가 알고 있을 수도 있겠지만 공개적으로 확실한 증거가 많이 있진 않긴 하죠. (FIM도 이런 Denosing Objective라고 생각해보면 사용해도 손해는 아니지만 특별히 성능이 나아지지도 않는다? 이런 느낌이기도 합니다.)

#llm 