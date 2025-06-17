https://arxiv.org/abs/2310.12773

Safe RLHF: Safe Reinforcement Learning from Human Feedback (Josef Dai, Xuehai Pan, Ruiyang Sun, Jiaming Ji, Xinbo Xu, Mickel Liu, Yizhou Wang, Yaodong Yang)

같은 데이터에 대해 Helpfulness와 Harmlessness 레이블을 독립적으로 수집하고, 수집한 Helpfulness 데이터로 Reward 모델을, Harmlessness 데이터로 Cost 모델을 만듭니다. 그리고 이 두 모델을 결합해서 Harmlessness라는 제약 조건 하에서 Helpfulness를 최대화하는 문제를 라그랑주 승수로 풀었네요. 굉장히 흥미롭습니다. 고정된 가중치로 결합하는 방법에 대한 유의미한 진전이 될 수 있지 않을까 싶네요.

https://github.com/PKU-Alignment/safe-rlhf

1M 규모의 Helpfulness, Harmlessness 데이터를 구축했다고 하고 공개 예정이라고 합니다. 데이터 구축과 RLHF 파이프라인을 세 번 돌리는 게 보통 작업은 아니었을 텐데...북경대가 대단하긴 하네요.

#safety #rl #alignment 