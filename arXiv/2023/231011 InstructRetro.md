https://arxiv.org/abs/2310.07713

InstructRetro: Instruction Tuning post Retrieval-Augmented Pretraining (Boxin Wang, Wei Ping, Lawrence McAfee, Peng Xu, Bo Li, Mohammad Shoeybi, Bryan Catanzaro)

NVIDIA에서 RETRO (https://arxiv.org/abs/2112.04426) 의 규모를 키워봤습니다. NVIDIA는 요즘 retrieval augmentation에 관심이 많네요. NVIDIA 쪽에서 자주 등장하는 GPT-43B를 사용해 100B 토큰에 대해 RETRO 학습을 추가로 한 다음, 그냥 100B 토큰에 대해 추가 학습시킨 모델과 비교해봤습니다.

흥미로운 점은 진행한 instruction tuning에서 retrieval encoder를 부분적으로만 사용하고, 추론 시에는 아예 사용하지 않았는데도 성능적 향상이 있었다는 것입니다. 논문의 제안대로라면 retrieval training이 단순히 retrieval 기능을 탑재시켜주는 것이 아니라 뭔가 다른 특성을 모델에 주입한다는 의미라는 것인데요. 흥미로운 포인트네요.

#retrieval #llm #continual_learning

# Links

# Links

