https://arxiv.org/abs/2507.02782

*Understanding and Improving Length Generalization in Recurrent Models* (Ricardo Buitrago Ruiz, Albert Gu)

> Recently, recurrent models such as state space models and linear attention have become popular due to their linear complexity in the sequence length. Thanks to their recurrent nature, in principle they can process arbitrarily long sequences, but their performance sometimes drops considerably beyond their training context lengths-i.e. they fail to length generalize. In this work, we provide comprehensive empirical and theoretical analysis to support the unexplored states hypothesis, which posits that models fail to length generalize when during training they are only exposed to a limited subset of the distribution of all attainable states (i.e. states that would be attained if the recurrence was applied to long sequences). Furthermore, we investigate simple training interventions that aim to increase the coverage of the states that the model is trained on, e.g. by initializing the state with Gaussian noise or with the final state of a different input sequence. With only 500 post-training steps ($\sim 0.1\%$ of the pre-training budget), these interventions enable length generalization for sequences that are orders of magnitude longer than the training context (e.g. $2k\longrightarrow 128k$) and show improved performance in long context tasks, thus presenting a simple and efficient way to enable robust length generalization in general recurrent models.

State Space Model의 길이 일반화 연구. 이전 시퀀스의 상태를 초기 상태로 사용해 다양한 상태를 접하게 하는 것으로 향상시킬 수 있다고. 사실 RNN 시절 LM을 학습하던 방법이죠.

SSM이 초기 상태에 민감하다는 이야기도 있었습니다만 (https://arxiv.org/abs/2406.07887) 어떨지 모르겠네요.

<english>
A study on length generalization of state space model. It insists that we can improve it by exposing model to various states by using state from previous sequences as an initial state. Actually it is the method used in training LM in RNN era.

There was a report that SSM is sensitive on initial states (https://arxiv.org/abs/2406.07887) thus I wonder this could 

#state-space-model #long-context