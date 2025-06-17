https://arxiv.org/abs/2506.05447

*Training Dynamics Underlying Language Model Scaling Laws: Loss Deceleration and Zero-Sum Learning* (Andrei Mircea, Supriyo Chakraborty, Nima Chitsazan, Irina Rish, Ekaterina Lobacheva)

> This work aims to understand how scaling improves language models, specifically in terms of training dynamics. We find that language models undergo loss deceleration early in training; an abrupt slowdown in the rate of loss improvement, resulting in piecewise linear behaviour of the loss curve in log-log space. Scaling up the model mitigates this transition by (1) decreasing the loss at which deceleration occurs, and (2) improving the log-log rate of loss improvement after deceleration. We attribute loss deceleration to a type of degenerate training dynamics we term zero-sum learning (ZSL). In ZSL, per-example gradients become systematically opposed, leading to destructive interference in per-example changes in loss. As a result, improving loss on one subset of examples degrades it on another, bottlenecking overall progress. Loss deceleration and ZSL provide new insights into the training dynamics underlying language model scaling laws, and could potentially be targeted directly to improve language models independent of scale. We make our code and artefacts available at: https://github.com/mirandrom/zsl

LM Loss의 감소 속도가 꺾이는 지점에서 어떤 일이 일어나는가에 대한 분석. 각 샘플의 그래디언트가 반대가 되어 모든 샘플들에 대해 Loss를 감소시킬 수 없게 되는 지점이라고 하네요.

<english>
Analysis on what happens where decreasing speed of LM loss deaccelerates. It is the point that gradient for each sample is oppose thus it is not possible to reduce loss for all samples.
</english>

#scaling-law #optimization 