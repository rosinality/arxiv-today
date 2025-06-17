https://arxiv.org/abs/2504.12463

*Dense Backpropagation Improves Training for Sparse Mixture-of-Experts* (Ashwinee Panda, Vatsal Baherwani, Zain Sarwar, Benjamin Therien, Supriyo Chakraborty, Tom Goldstein)

> Mixture of Experts (MoE) pretraining is more scalable than dense Transformer pretraining, because MoEs learn to route inputs to a sparse set of their feedforward parameters. However, this means that MoEs only receive a sparse backward update, leading to training instability and suboptimal performance. We present a lightweight approximation method that gives the MoE router a dense gradient update while continuing to sparsely activate its parameters. Our method, which we refer to as Default MoE, substitutes missing expert activations with default outputs consisting of an exponential moving average of expert outputs previously seen over the course of training. This allows the router to receive signals from every expert for each token, leading to significant improvements in training performance. Our Default MoE outperforms standard TopK routing in a variety of settings without requiring significant computational overhead. Code: https://github.com/vatsal0/default-moe.

MoE Router에 대한 Sparse Gradient를 Expert들의 평균 출력을 사용해 Dense Gradient로 전환한다는 아이디어. Sparse Mixer가 생각나네요. (https://arxiv.org/abs/2310.00811) 모델이 커질 때에도 차이가 얼마나 유지될지가 문제겠군요.

<english>
The idea of converting sparse gradient of MoE router into dense on by using average outputs of experts. It reminds me sparse mixer (https://arxiv.org/abs/2310.00811). Problem is whether the difference with baseline is sustained when model size is increased.
</english>

#moe 