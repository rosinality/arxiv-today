https://arxiv.org/abs/2503.07572

*Optimizing Test-Time Compute via Meta Reinforcement Fine-Tuning* (Yuxiao Qu, Matthew Y. R. Yang, Amrith Setlur, Lewis Tunstall, Edward Emanuel Beeching, Ruslan Salakhutdinov, Aviral Kumar)

> Training models to effectively use test-time compute is crucial for improving the reasoning performance of LLMs. Current methods mostly do so via fine-tuning on search traces or running RL with 0/1 outcome reward, but do these approaches efficiently utilize test-time compute? Would these approaches continue to scale as the budget improves? In this paper, we try to answer these questions. We formalize the problem of optimizing test-time compute as a meta-reinforcement learning (RL) problem, which provides a principled perspective on spending test-time compute. This perspective enables us to view the long output stream from the LLM as consisting of several episodes run at test time and leads us to use a notion of cumulative regret over output tokens as a way to measure the efficacy of test-time compute. Akin to how RL algorithms can best tradeoff exploration and exploitation over training, minimizing cumulative regret would also provide the best balance between exploration and exploitation in the token stream. While we show that state-of-the-art models do not minimize regret, one can do so by maximizing a dense reward bonus in conjunction with the outcome 0/1 reward RL. This bonus is the ''progress'' made by each subsequent block in the output stream, quantified by the change in the likelihood of eventual success. Using these insights, we develop Meta Reinforcement Fine-Tuning, or MRT, a new class of fine-tuning methods for optimizing test-time compute. MRT leads to a 2-3x relative gain in performance and roughly a 1.5x gain in token efficiency for math reasoning compared to outcome-reward RL.

Long CoT 모델의 생각의 단계들을 에피소드로 생각했을 때 에피소드들이 진행되는 것에 따라 정답 확률이 단조적으로 향상되지 않는다는 문제에 대한 지적. 이에 대해 에피소드들이 정답으로 진전되고 있는지를 보상으로 준다는 아이디어입니다.

Process Reward와 Outcome Reward는 계속해서 일종의 긴장 상태에 있네요.

<english>
Criticism on long CoT models when we consider each thought steps as an episode, probability of correct answer does not increases monotonically along with progression of episodes. For this problems give whether each episodes are progressing toward to correct anwers as a reward.

Process rewards and outcom rewards continuously in tension.
</english>

#rl #reasoning #reward 