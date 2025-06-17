https://arxiv.org/abs/2310.00898

Enable Language Models to Implicitly Learn Self-Improvement From Data (Ziqi Wang, Le Hou, Tianjian Lu, Yuexin Wu, Yunxuan Li, Hongkun Yu, Heng Ji)

LLM의 생성 결과를 개선하는 모델. preference를 사용해 비교적 좋지 않은 텍스트를 condition으로 해서 더 나은 텍스트를 생성하는 SFT와 좋은 텍스트와 좋지 않은 텍스트의 차이를 예측하는 RM으로 RLHF를 진행하는 군요. 이렇게 만든 모델로 모델 생성 결과를 개선할 수 있고, 이걸 반복적으로 적용할 수도 있습니다.

여담이지만 응답 하나를 받아 reward score를 만드는 모델보다 응답 둘을 입력으로 받아 비교하는 모델이 나을 수 있다는 것은 SLiC에서도 언급하고 있는 부분이긴 합니다. 다만 응답 토큰 수를 더 써야 한다는 게 문제인데...프롬프트는 공유하니 그럭저럭 할만 할 수도 있겠네요.

#alignment #rl 