https://arxiv.org/abs/2410.19034

*Mixture of Parrots: Experts improve memorization more than reasoning* (Samy Jelassi, Clara Mohri, David Brandfonbrener, Alex Gu, Nikhil Vyas, Nikhil Anand, David Alvarez-Melis, Yuanzhi Li, Sham M. Kakade, Eran Malach)

> The Mixture-of-Experts (MoE) architecture enables a significant increase in the total number of model parameters with minimal computational overhead. However, it is not clear what performance tradeoffs, if any, exist between MoEs and standard dense transformers. In this paper, we show that as we increase the number of experts (while fixing the number of active parameters), the memorization performance consistently increases while the reasoning capabilities saturate. We begin by analyzing the theoretical limitations of MoEs at reasoning. We prove that there exist graph problems that cannot be solved by any number of experts of a certain width; however, the same task can be easily solved by a dense model with a slightly larger width. On the other hand, we find that on memory-intensive tasks, MoEs can effectively leverage a small number of active parameters with a large number of experts to memorize the data. We empirically validate these findings on synthetic graph problems and memory-intensive closed book retrieval tasks. Lastly, we pre-train a series of MoEs and dense transformers and evaluate them on commonly used benchmarks in math and natural language. We find that increasing the number of experts helps solve knowledge-intensive tasks, but fails to yield the same benefits for reasoning tasks.

MoE가 지식의 기억에는 굉장히 효율적이지만 (증가한 파라미터가 Dense 모델의 파라미터 증가와 동등) 추론 능력에 대해서는 그렇지 않다는 결과. 추론 능력에는 임베딩 차원의 증가가 필요하다고 하는군요.

임베딩 차원의 증가 혹은 Attention 헤드의 증가와 동등한 효과를 낼 수 있는 Sparse 모델을 만들 수 있다면 좀 더 나아갈 수 있을지도 모르겠네요.

<english>
MoE is highly effective on memorizing knowledges (additional parameters incurred by MoE is directly equivalent to parameter of dense models.) but for reasonings it is less effective. The paper claims that you need to increase embedding dimensions for reasoning abilities.

I think we can may advance further if we can device sparse model that same effect with increasing embedding dimensions or attention heads.
</english>

#moe 