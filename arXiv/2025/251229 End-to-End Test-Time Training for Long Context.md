https://arxiv.org/abs/2512.23675

*End-to-End Test-Time Training for Long Context* (Arnuv Tandon, Karan Dalal, Xinhao Li, Daniel Koceja, Marcel Rød, Sam Buchanan, Xiaolong Wang, Jure Leskovec, Sanmi Koyejo, Tatsunori Hashimoto, Carlos Guestrin, Jed McCaleb, Yejin Choi, Yu Sun)

> We formulate long-context language modeling as a problem in continual learning rather than architecture design. Under this formulation, we only use a standard architecture -- a Transformer with sliding-window attention. However, our model continues learning at test time via next-token prediction on the given context, compressing the context it reads into its weights. In addition, we improve the model's initialization for learning at test time via meta-learning at training time. Overall, our method, a form of Test-Time Training (TTT), is End-to-End (E2E) both at test time (via next-token prediction) and training time (via meta-learning), in contrast to previous forms. We conduct extensive experiments with a focus on scaling properties. In particular, for 3B models trained with 164B tokens, our method (TTT-E2E) scales with context length in the same way as Transformer with full attention, while others, such as Mamba 2 and Gated DeltaNet, do not. However, similar to RNNs, TTT-E2E has constant inference latency regardless of context length, making it 2.7 times faster than full attention for 128K context. Our code is publicly available.

Next Token Prediction을 사용한 Test-Time Training. 초기 가중치가 Test-Time Training이 잘 작동하도록 학습되어야 하기 때문에 메타 러닝 문제가 됨. 흥미롭지만 규모 증대가 가능할지?

Test-Time Training with next token prediction. As initial weights should be optimized to allow test-time training to work well, this becomes a meta learning problem. Interesting, but would this be scalable?

#state-space-model #continual-learning 