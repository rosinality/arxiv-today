https://arxiv.org/abs/2506.02285

*Why Gradients Rapidly Increase Near the End of Training* (Aaron Defazio)

> During long-duration Large Language Model (LLM) training runs the gradient norm increases rapidly near the end of training. In this short note, we show that this increase is due to an unintended interaction between weight decay, normalization layers, and the learning rate schedule. We propose a simple correction that fixes this behavior while also resulting in lower loss values throughout training.

학습 과정의 그래디언트 노름의 증가가 LR 변화에 대해 Weight Decay가 고정되어 있기 때문이라는 분석. 그래서 Weight Decay를 LR에 비례하게 수정했는데 PaLM의 Weight Decay ∝ lr^2와 비슷하군요.

<english>
The analysis insist that the reasoning of increase in gradient norm during training is due to weight decay is fixed relative to changes in LR. Thus the paper suggest to change weight decay relative to LR, and in result, it is similar to Weight Decay ∝ lr^2 in PaLM.
</english>

#optimization 