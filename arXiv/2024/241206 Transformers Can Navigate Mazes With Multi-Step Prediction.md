https://arxiv.org/abs/2412.05117

*Transformers Can Navigate Mazes With Multi-Step Prediction* (Niklas Nolte, Ouail Kitouni, Adina Williams, Mike Rabbat, Mark Ibrahim)

> Despite their remarkable success in language modeling, transformers trained to predict the next token in a sequence struggle with long-term planning. This limitation is particularly evident in tasks requiring foresight to plan multiple steps ahead such as maze navigation. The standard next single token prediction objective, however, offers no explicit mechanism to predict multiple steps ahead - or revisit the path taken so far. Consequently, in this work we study whether explicitly predicting multiple steps ahead (and backwards) can improve transformers' maze navigation. We train parameter-matched transformers from scratch, under identical settings, to navigate mazes of varying types and sizes with standard next token prediction and MLM-U, an objective explicitly predicting multiple steps ahead and backwards. We find that MLM-U considerably improves transformers' ability to navigate mazes compared to standard next token prediction across maze types and complexities. We also find MLM-U training is 4x more sample efficient and converges 2x faster in terms of GPU training hours relative to next token training. Finally, for more complex mazes we find MLM-U benefits from scaling to larger transformers. Remarkably, we find transformers trained with MLM-U outperform larger transformers trained with next token prediction using additional supervision from A* search traces. We hope these findings underscore the promise of learning objectives to advance transformers' capacity for long-term planning.

Next Token Prediction 대신 MLM으로 앞뒤 N개 토큰 예측으로 학습시킬 때 미로 탐색 과제를 학습시킬 수 있다는 연구. 위의 연구와 비슷하군요. 추가적으로 RoPE의 정밀도 문제에 대해서도 언급하고 있네요. (https://arxiv.org/abs/2411.13476)

<english>
Research that transformer can learn maze exploration tasks when we train it with MLM that make model to predict N forward or backward tokens, instead of next token prediction. Additionally they mentions the numerical precision problem of RoPE. (https://arxiv.org/abs/2411.13476)
</english>

#transformer #autoregressive-model

# Links

[[241120 When Precision Meets Position.md]]