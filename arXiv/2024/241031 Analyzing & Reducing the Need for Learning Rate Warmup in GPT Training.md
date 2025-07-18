https://arxiv.org/abs/2410.23922

*Analyzing & Reducing the Need for Learning Rate Warmup in GPT Training* (Atli Kosson, Bettina Messmer, Martin Jaggi)

> Learning Rate Warmup is a popular heuristic for training neural networks, especially at larger batch sizes, despite limited understanding of its benefits. Warmup decreases the update size $\Delta \mathbf{w}_t = \eta_t \mathbf{u}_t$ early in training by using lower values for the learning rate $\eta_t$. In this work we argue that warmup benefits training by keeping the overall size of $\Delta \mathbf{w}_t$ limited, counteracting large initial values of $\mathbf{u}_t$. Focusing on small-scale GPT training with AdamW/Lion, we explore the following question: Why and by which criteria are early updates $\mathbf{u}_t$ too large? We analyze different metrics for the update size including the $\ell_2$-norm, resulting directional change, and impact on the representations of the network, providing a new perspective on warmup. In particular, we find that warmup helps counteract large angular updates as well as a limited critical batch size early in training. Finally, we show that the need for warmup can be significantly reduced or eliminated by modifying the optimizer to explicitly normalize $\mathbf{u}_t$ based on the aforementioned metrics.

LR Warmup이 필요한 이유는 무엇인가? 업데이트의 l2 Norm, 업데이트로 인한 파라미터의 각도 변화 및 Activation의 변화 측면에서 분석. Warmup이 이러한 변화가 지나치게 커지지 않도록 통제하는 측면에서 작동한다는 주장.

<english>
Why we need LR warmup? Analysis in aspect of l2 norm of update, and angular differences, activation changes after the updates. This paper says that warmup controls amount of these changes to not very large.
</english>

#optimizer 