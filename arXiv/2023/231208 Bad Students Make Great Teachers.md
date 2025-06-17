https://arxiv.org/abs/2312.05328

Bad Students Make Great Teachers:Active Learning Accelerates Large-Scale Visual Understanding (Talfan Evans, Shreya Pathak, Hamza Merzic, Jonathan Schwarz, Ryutaro Tanno, Olivier J. Henaff)

작은, 이미 학습된 모델과 온라인으로 학습하는 모델 하나를 두고 loss 차이를 통해 샘플을 선정하는 방식으로 active learning. 학습한 모델한테는 쉽지만 학습 중의 모델에는 어려운 샘플은 가치가 높다는 것이고, 둘 모두에게 쉽거나 둘 모두에게 어려운(어쩌면 레이블 에러) 샘플은 가치가 낮다는 식입니다.

큰 모델과 별개로 작은 모델 두 개를 갖고 가야 하기 때문에 실제 연산 효율성이 높은가가 문제가 되긴 합니다만, 일단 작은 모델로 샘플을 뽑아놓으면 여러 번 쓸 수 있으니 전반적으로는 괜찮을까 싶기도 하네요.

논문에서도 언급하는 DoReMi (https://arxiv.org/abs/2305.10429) 도 그렇고 샘플링 분포나 커리큘럼 또한 중요한 요소인데 어떤 영향을 미치는지 충분히 알려져 있지 않으니 이건 직접 실험해서 결과를 축적해야만 커버할 수 있는 영역일 듯 싶네요. 요새 instruction 데이터를 프리트레이닝에 넣는 것을 넘어 프리트레이닝 종반에 집중적으로 배치하고 있는 게 아니냐는 이야기도 나오는데 여하간 중요한 노하우일 것 같습니다.

#curriculum #active_learning

# Links

[[230517 DoReMi.md]]