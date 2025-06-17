https://arxiv.org/abs/2312.16682

Some things are more CRINGE than others: Preference Optimization with the Pairwise Cringe Loss (Jing Xu, Andrew Lee, Sainbayar Sukhbaatar, Jason Weston)

DPO 등에 대한 대안적 방법. Negative에 대해 Unlikelihood를 해버리면 다른 어떤 토큰들의 확률이 높아지는가에 대해서는 통제가 되지 않죠. 그래서 확률이 높은 Top-K 토큰을 Positive로 설정 학습하는 방법입니다. 추가적으로 Positive와 Negative 사이의 마진이 작을 때에만 Loss를 적용하는 것과 Reward Model을 사용해 반복적으로 학습하는 방법을 시도했네요.

#rlhf 