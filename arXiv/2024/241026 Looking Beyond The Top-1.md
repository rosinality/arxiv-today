https://arxiv.org/abs/2410.20210

*Looking Beyond The Top-1: Transformers Determine Top Tokens In Order* (Daria Lioubashevski, Tomer Schlank, Gabriel Stanovsky, Ariel Goldstein)

> Understanding the inner workings of Transformers is crucial for achieving more accurate and efficient predictions. In this work, we analyze the computation performed by Transformers in the layers after the top-1 prediction has become fixed, which has been previously referred to as the "saturation event". We expand the concept of saturation events for top-k tokens, demonstrating that similar saturation events occur across language, vision, and speech models. We find that these saturation events happen in order of the corresponding tokens' ranking, i.e., the model first decides on the top ranking token, then the second highest ranking token, and so on. This phenomenon seems intrinsic to the Transformer architecture, occurring across different architectural variants (decoder-only, encoder-only, and to a lesser extent full-Transformer), and even in untrained Transformers. We propose an underlying mechanism of task transition for this sequential saturation, where task k corresponds to predicting the k-th most probable token, and the saturation events are in fact discrete transitions between the tasks. In support of this we show that it is possible to predict the current task from hidden layer embedding. Furthermore, using an intervention method we demonstrate that we can cause the model to switch from one task to the next. Finally, leveraging our findings, we introduce a novel token-level early-exit strategy, which surpasses existing methods in balancing performance and efficiency.

트랜스포머 내에서 Top-1 토큰을 결정하고 이 결정이 바뀌지 않는 지점이 있고, 그 다음으로 Top-2가 결정되는 식으로 순서대로 토큰 순위가 결정된다는 분석. 마치 과제를 순차적으로 해결하듯 Top-1 토큰 결정 과제를 수행 완료 했다는 신호가 발생하면 Top-2 결정 과제를 수행하는 식으로 작동하는 것 같다는 분석이네요.

<english>
In transformer there a point that top-1 token is determined and does not changed after that, and then top-2 token is determined, and overall rank of tokens are predicted in this sequential manner. The authors suspect that like doing tasks sequentially, after the task that predicting top-1 token and layers make a signal it is done, then later layers doing the task for predicting top-2.
</english>

#transformer 