https://arxiv.org/abs/2411.12537

*Unlocking State-Tracking in Linear RNNs Through Negative Eigenvalues* (Riccardo Grazzi, Julien Siems, Jörg K.H. Franke, Arber Zela, Frank Hutter, Massimiliano Pontil)

> Linear Recurrent Neural Networks (LRNNs) such as Mamba, RWKV, GLA, mLSTM, and DeltaNet have emerged as efficient alternatives to Transformers in large language modeling, offering linear scaling with sequence length and improved training efficiency. However, LRNNs struggle to perform state-tracking which may impair performance in tasks such as code evaluation or tracking a chess game. Even parity, the simplest state-tracking task, which non-linear RNNs like LSTM handle effectively, cannot be solved by current LRNNs. Recently, Sarrof et al. (2024) demonstrated that the failure of LRNNs like Mamba to solve parity stems from restricting the value range of their diagonal state-transition matrices to $[0, 1]$ and that incorporating negative values can resolve this issue. We extend this result to non-diagonal LRNNs, which have recently shown promise in models such as DeltaNet. We prove that finite precision LRNNs with state-transition matrices having only positive eigenvalues cannot solve parity, while complex eigenvalues are needed to count modulo $3$. Notably, we also prove that LRNNs can learn any regular language when their state-transition matrices are products of identity minus vector outer product matrices, each with eigenvalues in the range $[-1, 1]$. Our empirical results confirm that extending the eigenvalue range of models like Mamba and DeltaNet to include negative values not only enables them to solve parity but consistently improves their performance on state-tracking tasks. Furthermore, pre-training LRNNs with an extended eigenvalue range for language modeling achieves comparable performance and stability while showing promise on code and math data. Our work enhances the expressivity of modern LRNNs, broadening their applicability without changing the cost of training or inference.

Linear RNN이 병렬화를 추구하면서 표현력을 희생했다는 연구들이 있었죠. (https://arxiv.org/abs/2404.08819, https://arxiv.org/abs/2405.17394) 여기서는 Linear RNN의 표현력을 제약하는 것이 Transition 행렬의 고윳값이 양수라는 것 때문이라고 분석했네요. 따라서 고윳값이 음수가 될 수 있도록 바꾸면 표현력이 향상됩니다.

<english>
There was studies shows that linear RNNs sacrificed representational capacity while pursuing parallelization. (https://arxiv.org/abs/2404.08819, https://arxiv.org/abs/2405.17394) This study says that limitation of representational for linear RNNs is came from the fact that eigenvalue of transition matrix is positive. So if we change the formulation to allow negative eigenvalues then we can improve representational capacity of linear RNNs.
</english>

#state-space-model

# Links

[[240412 The Illusion of State in State-Space Models.md]]