https://arxiv.org/abs/2404.08819

*The Illusion of State in State-Space Models* (William Merrill, Jackson Petty, Ashish Sabharwal)

> State-space models (SSMs) have emerged as a potential alternative architecture for building large language models (LLMs) compared to the previously ubiquitous transformer architecture. One theoretical weakness of transformers is that they cannot express certain kinds of sequential computation and state tracking (Merrill and Sabharwal, 2023), which SSMs are explicitly designed to address via their close architectural similarity to recurrent neural networks (RNNs). But do SSMs truly have an advantage (over transformers) in expressive power for state tracking? Surprisingly, the answer is no. Our analysis reveals that the expressive power of SSMs is limited very similarly to transformers: SSMs cannot express computation outside the complexity class $\mathsf{TC}^0$. In particular, this means they cannot solve simple state-tracking problems like permutation composition. It follows that SSMs are provably unable to accurately track chess moves with certain notation, evaluate code, or track entities in a long narrative. To supplement our formal analysis, we report experiments showing that Mamba-style SSMs indeed struggle with state tracking. Thus, despite its recurrent formulation, the "state" in an SSM is an illusion: SSMs have similar expressiveness limitations to non-recurrent models like transformers, which may fundamentally limit their ability to solve real-world state-tracking problems.

체스 기보를 입력으로 받아 체스판의 최종 상태를 예측하는 것과 같은 상태 추적 과제에 대해서 State Space Model이 Transformer와 비슷하다는 분석. 가장 큰 문제는 Hidden State에 대한 Projection이 고정된 행렬이거나 게이트를 사용하는 경우에는 대각 행렬이라는 것이 문제입니다. 이런 제약을 걸면 표현력에 한계가 생긴다는 것이죠.

이에 대응하려면 다음 Hidden State를 계산하는 과정에 Nonlinearity를 주거나 게이트 행렬이 대각 행렬이라는 제약을 풀어야 합니다. 과거의 RNN과 비슷해지면서 병렬화와 계산 효율성에서 문제가 크죠.

병렬화나 계산 효율성과 표현력에는 어쩔 수 없는 트레이드오프가 있는 것이 아닌가 하는 생각도 듭니다.

#state-space-model 