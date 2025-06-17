https://arxiv.org/abs/2503.10799

*Fixed-Point RNNs: From Diagonal to Dense in a Few Iterations* (Sajad Movahedi, Felix Sarnthein, Nicola Muca Cirone, Antonio Orvieto)

> Linear recurrent neural networks (RNNs) and state-space models (SSMs) such as Mamba have become promising alternatives to softmax-attention as sequence mixing layers in Transformer architectures. Current models, however, do not exhibit the full state-tracking expressivity of RNNs because they rely on channel-wise (i.e. diagonal) sequence mixing. In this paper, we propose to compute a dense linear RNN as the fixed-point of a parallelizable diagonal linear RNN in a single layer. We explore mechanisms to improve its memory and state-tracking abilities in practice, and achieve state-of-the-art results on the commonly used toy tasks $A_5$, $S_5$, copying, and modular arithmetics. We hope our results will open new avenues to more expressive and efficient sequence mixers.

고정점을 갖도록 디자인한 Linear RNN을 사용해서 Diagonal Transition Linear RNN의 표현력 제약을 해소한 시도.

<english>
An attempt of relieving representational limits of diagonal transition linear RNN by using linear RNN designed to have fixed point.
</english>

#state-space-model 