https://arxiv.org/abs/2501.04697

*Grokking at the Edge of Numerical Stability* (Lucas Prieto, Melih Barsbey, Pedro A.M. Mediano, Tolga Birdal)

> Grokking, the sudden generalization that occurs after prolonged overfitting, is a surprising phenomenon challenging our understanding of deep learning. Although significant progress has been made in understanding grokking, the reasons behind the delayed generalization and its dependence on regularization remain unclear. In this work, we argue that without regularization, grokking tasks push models to the edge of numerical stability, introducing floating point errors in the Softmax function, which we refer to as Softmax Collapse (SC). We demonstrate that SC prevents grokking and that mitigating SC enables grokking without regularization. Investigating the root cause of SC, we find that beyond the point of overfitting, the gradients strongly align with what we call the na\"ive loss minimization (NLM) direction. This component of the gradient does not alter the model's predictions but decreases the loss by scaling the logits, typically by scaling the weights along their current direction. We show that this scaling of the logits explains the delay in generalization characteristic of grokking and eventually leads to SC, halting further learning. To validate our hypotheses, we introduce two key contributions that address the challenges in grokking tasks: StableMax, a new activation function that prevents SC and enables grokking without regularization, and $\perp$Grad, a training algorithm that promotes quick generalization in grokking tasks by preventing NLM altogether. These contributions provide new insights into grokking, elucidating its delayed generalization, reliance on regularization, and the effectiveness of existing grokking-inducing methods. Code for this paper is available at https://github.com/LucasPrietoAl/grokking-at-the-edge-of-numerical-stability.

Grokking이 일어나려면 Regularization이 필요한 이유에 대한 분석. 모델이 100% 정확도를 나타내는 상황에서도 Loss를 낮추기 위해 Logit의 크기를 계속 키우도록 학습되고 Logit이 일정 이상 커지면 Softmax의 그래디언트가 0이 되기 때문이라는 분석.

<english>
Analysis on why we need regularization to make grokking happen. This paper says that model trained to increase logit for reducing the loss even when it has 100% accuracy, and gradient of softmax became 0 when scale logit became larger than certain threshold.
</english>

#grokking  #optimizer 