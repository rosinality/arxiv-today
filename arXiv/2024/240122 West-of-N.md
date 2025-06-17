https://arxiv.org/abs/2401.12086

*West-of-N: Synthetic Preference Generation for Improved Reward Modeling* (Alizée Pace, Jonathan Mallinson, Eric Malmi, Sebastian Krause, Aliaksei Severyn)

> The success of reinforcement learning from human feedback (RLHF) in language model alignment is strongly dependent on the quality of the underlying reward model. In this paper, we present a novel approach to improve reward model quality by generating synthetic preference data, thereby augmenting the training dataset with on-policy, high-quality preference pairs. Motivated by the promising results of Best-of-N sampling strategies in language model training, we extend their application to reward model training. This results in a self-training strategy to generate preference pairs by selecting the best and worst candidates in a pool of responses to a given query. Empirically, we find that this approach improves the performance of any reward model, with an effect comparable to the addition of a similar quantity of human preference data. This work opens up new avenues of research for improving RLHF for language model alignment, by offering synthetic preference generation as a solution to reward modeling challenges.

West = Best + Worst입니다. 얼마 전에 나온 Self-Rewarding Language Models (https://arxiv.org/abs/2401.10020) 와 비슷하게 약간의 Preference Pair로 모델을 학습해서 Reward Model로의 기능을 하게 한 다음 모델 샘플을 이 Reward Model로 분류해서 데이터셋을 구축하는 방법입니다.

여기서의 차이는 두 개 샘플만 뽑는 대신 샘플을 여러 개 뽑아서 Preference의 정도가 가장 다른 페어를 학습에 쓴다는 것이겠네요. 모델의 성능에 따른 노이즈를 줄이기 위함입니다.

샘플을 여러 개 뽑고 그 안에서 비교한다는 점에서는 RSO (https://arxiv.org/abs/2309.06657) 가 떠오르기도 하고 그렇네요. 물론 여러 이터레이션을 도는 것도 가능합니다. 이런 방법은 LM이 강해질수록 더 효과적일 것이라 아주 강력한 수준의 모델에서 어디까지 가능할지 궁금해지네요.

#reward-model #rlhf #alignment

# Links

[[240118 Self-Rewarding Language Models.md]]