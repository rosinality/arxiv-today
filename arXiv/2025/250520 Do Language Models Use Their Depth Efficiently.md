https://arxiv.org/abs/2505.13898

*Do Language Models Use Their Depth Efficiently?* (Róbert Csordás, Christopher D. Manning, Christopher Potts)

> Modern LLMs are increasingly deep, and depth correlates with performance, albeit with diminishing returns. However, do these models use their depth efficiently? Do they compose more features to create higher-order computations that are impossible in shallow models, or do they merely spread the same kinds of computation out over more layers? To address these questions, we analyze the residual stream of the Llama 3.1 and Qwen 3 family of models. We find: First, comparing the output of the sublayers to the residual stream reveals that layers in the second half contribute much less than those in the first half, with a clear phase transition between the two halves. Second, skipping layers in the second half has a much smaller effect on future computations and output predictions. Third, for multihop tasks, we are unable to find evidence that models are using increased depth to compose subresults in examples involving many hops. Fourth, we seek to directly address whether deeper models are using their additional layers to perform new kinds of computation. To do this, we train linear maps from the residual stream of a shallow model to a deeper one. We find that layers with the same relative depth map best to each other, suggesting that the larger model simply spreads the same computations out over its many layers. All this evidence suggests that deeper models are not using their depth to learn new kinds of computation, but only using the greater depth to perform more fine-grained adjustments to the residual. This may help explain why increasing scale leads to diminishing returns for stacked Transformer architectures.

트랜스포머 LM이 레이어들을 효과적으로 사용하지 않는 것 같다는 분석. 깊은 모델은 얕은 모델을 잡아 늘린 것과 비슷한 방식으로 작동하고 레이어들이 출력 결과의 세부 조정을 위해 사용되고 있다고 하네요.

LM이라는 학습 목표의 문제일 수도 있고 Pre Norm 혹은 Layer Reuse 같은 아키텍처 관련 문제일 수도 있겠죠. 이를 해소할 수 있다면 LM의 성능이 크게 달라질까요.

<english>
An analysis insists that transformer LM does not effectively use layers. Deeper models work similary stretched-out shallower models, and many layers used for fine adjustment for outputs.

It maybe the problem of training objective of LM, and maybe related to architectural problems like pre norm or layer reuse. If we resolve this, then would it increase performance of LM greatly?
</english>

#transformer #lm 