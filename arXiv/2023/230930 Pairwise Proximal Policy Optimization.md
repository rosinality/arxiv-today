https://arxiv.org/abs/2310.00212

Pairwise Proximal Policy Optimization: Harnessing Relative Feedback for LLM Alignment (Tianhao Wu, Banghua Zhu, Ruoyu Zhang, Zhaojin Wen, Kannan Ramchandran, Jiantao Jiao)

PPO의 문제로 reward의 shift에 대해 invariant 하지 않다는 것과 샘플 단위가 아니라 토큰 단위로 학습한다는 것을 들고 있네요. 이에 대한 대안으로 샘플 두 개를 뽑고 이 샘플 둘에 대한 reward의 차이에 의존하는 형태의 방법을 만들었습니다. PPO 대신 바로 적용해볼 수 있을 것 같은 형태의 알고리즘이네요.

Reward의 차이를 사용하는 것을 지향하는 방법과도 (https://arxiv.org/abs/2310.00898) 결합이 가능할까요? 흥미로운 문제일 듯 싶습니다.

#alignment #rl

# Links

[[231002 Enable Language Models to Implicitly Learn Self-Improvement From Data.md]]