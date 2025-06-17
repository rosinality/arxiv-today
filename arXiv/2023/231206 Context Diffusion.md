https://arxiv.org/abs/2312.03584

Context Diffusion: In-Context Aware Image Generation (Ivona Najdenkoska, Animesh Sinha, Abhimanyu Dubey, Dhruv Mahajan, Vignesh Ramanathan, Filip Radenovic)

diffusion으로 in-context learning 하기. 결과적으로는 query와 context 이미지에 대해 conditional 하게 생성한다는 느낌이죠. context로 스타일을 주고 query로 스케치를 준 다음 이미지를 생성한다는 등은 좀 평범하지만(?) context로 segmentation map을 주고 query로 이미지를 줘서 segmentation을 한다거나 하는 시나리오는 흥미롭지 않나 싶습니다.

vision 쪽에서는 vision task들을 사용해서 모델을 구성하는 접근이 여전히 통용되고 있네요. language 쪽과의 차이가 아닐까 싶습니다. (생각해보면 프리트레이닝 시점에 instruction data라는 이름의 multitask 데이터를 추가하는 것이 흔한 것을 보면 language 쪽도 비슷할지도 모르겠습니다.)

#in_context_learning #diffusion 