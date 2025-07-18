https://arxiv.org/abs/2401.04056

*A Minimaximalist Approach to Reinforcement Learning from Human Feedback* (Gokul Swamy, Christoph Dann, Rahul Kidambi, Zhiwei Steven Wu, Alekh Agarwal)

> We present Self-Play Preference Optimization (SPO), an algorithm for reinforcement learning from human feedback. Our approach is minimalist in that it does not require training a reward model nor unstable adversarial training and is therefore rather simple to implement. Our approach is maximalist in that it provably handles non-Markovian, intransitive, and stochastic preferences while being robust to the compounding errors that plague offline approaches to sequential prediction. To achieve the preceding qualities, we build upon the concept of a Minimax Winner (MW), a notion of preference aggregation from the social choice theory literature that frames learning from preferences as a zero-sum game between two policies. By leveraging the symmetry of this game, we prove that rather than using the traditional technique of dueling two policies to compute the MW, we can simply have a single agent play against itself while maintaining strong convergence guarantees. Practically, this corresponds to sampling multiple trajectories from a policy, asking a rater or preference model to compare them, and then using the proportion of wins as the reward for a particular trajectory. We demonstrate that on a suite of continuous control tasks, we are able to learn significantly more efficiently than reward-model based approaches while maintaining robustness to the intransitive and stochastic preferences that frequently occur in practice when aggregating human judgments.

Reward 대신 Preference 기반으로 Minimax Winner를 산출하기 위한 방법. Nash Learning (https://arxiv.org/abs/2312.00886) 과 연결되는군요. 기본적으로 Reward보다 Preference가 더 바람직하다고 보고, Minimax Solution을 모델 하나로 학습하기 위한 방법입니다.

알고리즘을 보면 샘플 Trajectory를 큐에 넣고 새로운 샘플을 만들면서 큐 내의 샘플과 Preference를 계산해 Win rate를 Reward로 사용하는 방식입니다. 일단 Continuous Control 문제에 대한 테스트만 있긴 합니다만 Preference 기반 방법들이 계속 나오고 있는 걸 보면 관심이 가네요.

#rlhf

# Links

[[231201 Nash Learning from Human Feedback.md]]