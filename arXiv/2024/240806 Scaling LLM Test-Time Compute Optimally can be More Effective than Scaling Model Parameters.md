https://arxiv.org/abs/2408.03314

*Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters* (Charlie Snell, Jaehoon Lee, Kelvin Xu, Aviral Kumar)

> Enabling LLMs to improve their outputs by using more test-time computation is a critical step towards building generally self-improving agents that can operate on open-ended natural language. In this paper, we study the scaling of inference-time computation in LLMs, with a focus on answering the question: if an LLM is allowed to use a fixed but non-trivial amount of inference-time compute, how much can it improve its performance on a challenging prompt? Answering this question has implications not only on the achievable performance of LLMs, but also on the future of LLM pretraining and how one should tradeoff inference-time and pre-training compute. Despite its importance, little research attempted to understand the scaling behaviors of various test-time inference methods. Moreover, current work largely provides negative results for a number of these strategies. In this work, we analyze two primary mechanisms to scale test-time computation: (1) searching against dense, process-based verifier reward models; and (2) updating the model's distribution over a response adaptively, given the prompt at test time. We find that in both cases, the effectiveness of different approaches to scaling test-time compute critically varies depending on the difficulty of the prompt. This observation motivates applying a "compute-optimal" scaling strategy, which acts to most effectively allocate test-time compute adaptively per prompt. Using this compute-optimal strategy, we can improve the efficiency of test-time compute scaling by more than 4x compared to a best-of-N baseline. Additionally, in a FLOPs-matched evaluation, we find that on problems where a smaller base model attains somewhat non-trivial success rates, test-time compute can be used to outperform a 14x larger model.

추론 시점의 연산 투입의 효과에 대한 연구가 많이 나오고 있군요. 서치를 통해서 LLM을 개선하고자 하는 흐름이 계속 있었으니 자연스러운 일이긴 합니다.

여기서는 추론 시점의 연산 투입을 두 가지 축에서 생각합니다. 1. 모델의 샘플링 결과를 Verifier로 분류하는 방법. 2. 프롬프트를 바꿔 모델의 샘플 분포를 바꾸는 방법.

1번에 대해서는 PRM을 만들고 빔 서치 같은 다양한 방법을 사용해 연산 사용량의 증가에 따른 성능 향상을 분석했습니다. 여기서 핵심은 문제의 난이도에 따라 최적 탐색 방법과 탐색량이 달라진다는 것입니다. (난이도가 높아질수록 더 강력한 검색 방법의 효과가 증가.)

2번에 대해서는 이전 샘플링 결과를 Revise하는 모델을 학습시켰습니다. Revision은 Sequential한 과정이기에 Parallel하게 샘플링한 다음 Verifier를 사용하는 방향의 일반화를 시도했습니다. 그리고 여기에서도 문제 난이도에 따른 Sequential vs Parallel의 최적 비율이 달랐다고 하네요. 문제가 쉬울수록 Sequential의 비중이 높다고 합니다.

그렇다면 프리트레이닝과 추론에 대한 투입 연산량의 트레이드오프는? 문제의 난이도가 높아지고 추론을 많이 할 것이라면 프리트레이닝에 연산을 투입하는 것이 좋다는 이야기를 합니다. 반대라면 추론 시점에 연산을 투입하는 것이 가능하죠.

이 트레이드오프가 문제의 난이도에 따라 달라진다는 것이 가장 흥미로운 부분일 듯 합니다.

#search 