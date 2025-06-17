https://arxiv.org/abs/2312.00886

Nash Learning from Human Feedback (Rémi Munos, Michal Valko, Daniele Calandriello, Mohammad Gheshlaghi Azar, Mark Rowland, Daniel Guo, Yunhao Tang, Matthieu Geist, Thomas Mésnard, Andrea Michi, Marco Selvi, Sertan Girgin, Nikola Momchev, Olivier Bachem, Daniel J. Mankowitz, Doina Precup, Bilal Piot)

https://x.com/misovalko/status/1731696738379936160

Bradley-Terry 모델을 Preference 모델, 즉 두 개의 응답을 받아 선호하는 응답을 분류하는 모델로 바꾸고 이 Preference에 대한 내시 균형을 목표로 최적화하는 방법. 내시 균형 상태에서는 다른 모든 Policy 보다 선호되는 Policy에 도달하게 되죠.

Bradley-Terry 모델이 아니라 Preference 모델을 선택한 것이 중요한 포인트일 것 같은데, 여기서는 x > y, y > z, z > x를 모델링 할 수 있는 것 (non transitivity) 을 오히려 장점이라고 보고 있습니다. 사람의 다양한 선호를 고려할 수 있다는 것, 그리고 샘플링 분포에 의존하지 않는다고 말하고 있네요.

Preference 모델이 더 나을 수 있지 않은가라는 이야기는 SLiC-HF (https://arxiv.org/abs/2305.10425) 에서도 나왔었죠. 문제 의식과 방법은 완전히 다르지만 응답 페어를 쓰는 접근도 생각나네요. (https://arxiv.org/abs/2310.00212)

#alignment #rlhf 

[[230517 SLiC-HF]]
[[230930 Pairwise Proximal Policy Optimization]]

# Links

[[230517 SLiC-HF.md]]