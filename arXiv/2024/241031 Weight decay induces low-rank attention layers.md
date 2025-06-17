https://arxiv.org/abs/2410.23819

*Weight decay induces low-rank attention layers* (Seijin Kobayashi, Yassir Akram, Johannes Von Oswald)

> The effect of regularizers such as weight decay when training deep neural networks is not well understood. We study the influence of weight decay as well as $L2$-regularization when training neural network models in which parameter matrices interact multiplicatively. This combination is of particular interest as this parametrization is common in attention layers, the workhorse of transformers. Here, key-query, as well as value-projection parameter matrices, are multiplied directly with each other: $W_K^TW_Q$ and $PW_V$. We extend previous results and show on one hand that any local minimum of a $L2$-regularized loss of the form $L(AB^\top) + \lambda (\|A\|^2 + \|B\|^2)$ coincides with a minimum of the nuclear norm-regularized loss $L(AB^\top) + \lambda\|AB^\top\|_*$, and on the other hand that the 2 losses become identical exponentially quickly during training. We thus complement existing works linking $L2$-regularization with low-rank regularization, and in particular, explain why such regularization on the matrix product affects early stages of training. Based on these theoretical insights, we verify empirically that the key-query and value-projection matrix products $W_K^TW_Q, PW_V$ within attention layers, when optimized with weight decay, as usually done in vision tasks and language modelling, indeed induce a significant reduction in the rank of $W_K^TW_Q$ and $PW_V$, even in fully online training. We find that, in accordance with existing work, inducing low rank in attention matrix products can damage language model performance, and observe advantages when decoupling weight decay in attention layers from the rest of the parameters.

Attention 레이어의 Linear Weight에 대한 Weight Decay가 Attention Logit 등에 대해 Low Rank Regularization을 부과할 수 있다는 주장. 따라서 Attention에 대해서는 다른 FFN보다 낮은 Weight Decay를 사용할 필요가 있을 수 있다는 아이디어네요.

<english>
By applying weight decay on linear weights from attention layer it could induce low rank regularization on attention logits. So it may need to use lower weight decay on attention layers compared to FFNs.
</english>

#transformer #regularization 