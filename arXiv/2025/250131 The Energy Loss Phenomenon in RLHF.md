https://arxiv.org/abs/2501.19358

*The Energy Loss Phenomenon in RLHF: A New Perspective on Mitigating Reward Hacking* (Yuchun Miao, Sen Zhang, Liang Ding, Yuqi Zhang, Lefei Zhang, Dacheng Tao)

> This work identifies the Energy Loss Phenomenon in Reinforcement Learning from Human Feedback (RLHF) and its connection to reward hacking. Specifically, energy loss in the final layer of a Large Language Model (LLM) gradually increases during the RL process, with an excessive increase in energy loss characterizing reward hacking. Beyond empirical analysis, we further provide a theoretical foundation by proving that, under mild conditions, the increased energy loss reduces the upper bound of contextual relevance in LLMs, which is a critical aspect of reward hacking as the reduced contextual relevance typically indicates overfitting to reward model-favored patterns in RL. To address this issue, we propose an Energy loss-aware PPO algorithm (EPPO) which penalizes the increase in energy loss in the LLM's final layer during reward calculation to prevent excessive energy loss, thereby mitigating reward hacking. We theoretically show that EPPO can be conceptually interpreted as an entropy-regularized RL algorithm, which provides deeper insights into its effectiveness. Extensive experiments across various LLMs and tasks demonstrate the commonality of the energy loss phenomenon, as well as the effectiveness of \texttt{EPPO} in mitigating reward hacking and improving RLHF performance.

RLHF 과정에서 마지막 레이어의 입력과 출력의 차이(Energy Loss)가 증가하는데, 이 Energy Loss의 급격한 증가가 Reward Hacking과 관련이 있다는 연구. 이를 억제해서 Reward Hacking을 감소시키려는 시도를 했습니다. 결과적으로는 Entropy regularization과 이어지네요.

<english>
The study insist that energy loss which is the difference between input and output of last layer increases during RLHF, and drastic increase of it is related with reward hacking. They tried to reduce reward hacking by suppressing it. Consequently it has connection with entropy regularization.
</english>

#alignment #rlhf 