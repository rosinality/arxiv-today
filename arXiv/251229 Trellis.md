https://arxiv.org/abs/2512.23852

*Trellis: Learning to Compress Key-Value Memory in Attention Models* (Mahdi Karami, Ali Behrouz, Praneeth Kacham, Vahab Mirrokni)

> Transformers, while powerful, suffer from quadratic computational complexity and the ever-growing Key-Value (KV) cache of the attention mechanism. This paper introduces Trellis, a novel Transformer architecture with bounded memory that learns how to compress its key-value memory dynamically at test time. Trellis replaces the standard KV cache with a fixed-size memory and train a two-pass recurrent compression mechanism to store new keys and values into memory. To achieve this, it leverages an online gradient descent procedure with a forget gate, enabling the compressed memory to be updated recursively while learning to retain important contextual information from incoming tokens at test time. Extensive experiments on language modeling, common-sense reasoning, recall-intensive tasks, and time series show that the proposed architecture outperforms strong baselines. Notably, its performance gains increase as the sequence length grows, highlighting its potential for long-context applications.

비선형 Recurrence를 사용하는 Test-Time Training과 L2 정규화를 결합한 Slot Attention. 저자들은 이런 형태의 아키텍처에 대해 굉장히 많이 탐색해왔는데 최종적으로 하나의 아키텍처로 수렴하게 될지 궁금.

Slot attention using Test-Time Training with nonlinear recurrence and L2 regularization. The authors explored various possibilities of these architectures. Will this converge to one architecture?

#state-space-model 