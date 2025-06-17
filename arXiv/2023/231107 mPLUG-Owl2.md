https://arxiv.org/abs/2311.04257

mPLUG-Owl2: Revolutionizing Multi-modal Large Language Model with Modality Collaboration (Qinghao Ye, Haiyang Xu, Jiabo Ye, Ming Yan, Haowei Liu, Qi Qian, Ji Zhang, Fei Huang, Jingren Zhou)

LM에 multimodal 입력을 끼워넣는 접근으로 modality에 간섭을 유발하거나 LM을 얼려놓아 텍스트 성능을 그대로 보존하는 것을 목표로 하는 것이 아니라 오히려 상승 효과를 내도록 할 수 없는가에 대한 연구.

프리트레이닝 시점에서는 이미지 토큰에 대해서는 다른 layer normalization과 key/value projection을 학습하고 나머지는 공유합니다. instruction tuning에서 전체 모델을 학습시킨다는 것이 차이겠네요. 추가적으로 vision encoder도 프리트레이닝과 파인튜닝 시점에서 모두 학습시킵니다.

이걸 통해서 텍스트 과제에 대해서도 성능 향상을 발생시킬 수 있었다는 것이 주요 결과군요. 흥미롭네요. 점점 더 얼린 인코더와 디코더를 쓰는 대신 서로 다른 modality를 위해 다른 weight를 주어야 한다는 아이디어가 많이 나오는 듯 한데 (https://arxiv.org/abs/2311.03079, https://arxiv.org/abs/2311.02684) 다르게 보면 scratch training의 의미가 점점 드러나고 있는 듯한 느낌입니다.

#vision-language #multimodal

# Links

[[231106 CogVLM.md]]
[[231105 Octavius.md]]