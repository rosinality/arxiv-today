https://arxiv.org/abs/2408.10189

*Transformers to SSMs: Distilling Quadratic Knowledge to Subquadratic Models* (Aviv Bick, Kevin Y. Li, Eric P. Xing, J. Zico Kolter, Albert Gu)

> Transformer architectures have become a dominant paradigm for domains like language modeling but suffer in many inference settings due to their quadratic-time self-attention. Recently proposed subquadratic architectures, such as Mamba, have shown promise, but have been pretrained with substantially less computational resources than the strongest Transformer models. In this work, we present a method that is able to distill a pretrained Transformer architecture into alternative architectures such as state space models (SSMs). The key idea to our approach is that we can view both Transformers and SSMs as applying different forms of mixing matrices over the token sequences. We can thus progressively distill the Transformer architecture by matching different degrees of granularity in the SSM: first matching the mixing matrices themselves, then the hidden units at each block, and finally the end-to-end predictions. Our method, called MOHAWK, is able to distill a Mamba-2 variant based on the Phi-1.5 architecture (Phi-Mamba) using only 3B tokens and a hybrid version (Hybrid Phi-Mamba) using 5B tokens. Despite using less than 1% of the training data typically used to train models from scratch, Phi-Mamba boasts substantially stronger performance compared to all past open-source non-Transformer models. MOHAWK allows models like SSMs to leverage computational resources invested in training Transformer-based architectures, highlighting a new avenue for building such models.

Transformer에서 State Space Model로 Distillation. Attention도 SSM도 Sequence Mixing의 문제로 생각하기에 이 두 Mixing 행렬에 대한 Distillation이 기본이 되네요.

Local Attention과 Global Attention의 조합이 Long Context에서 Attention의 추론 부담을 줄여주는 방법으로 정립되고 있는 듯 해서 추론 성능을 위해 SSM을 사용할 동인이 줄어든 것 같긴 합니다.

#distillation #state-space-model 