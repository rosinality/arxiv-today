https://arxiv.org/abs/2506.12543

*Is your batch size the problem? Revisiting the Adam-SGD gap in language modeling* (Teodora Srećković, Jonas Geiping, Antonio Orvieto)

> Adam is known to perform significantly better than Stochastic Gradient Descent (SGD) in language models, a phenomenon for which a number of explanations have been proposed. In this work, we revisit this "optimizer gap" through a series of comprehensively tuned baseline training runs for language modeling with Transformers. We exhaustively study how momentum, gradient clipping, and batch size affect the gap between SGD and Adam. Our empirical findings show that SGD with momentum can actually perform similarly to Adam in small-batch settings, if tuned correctly. We revisit existing explanations for Adam's advantage, including heavy-tailed class imbalance, directional sharpness, and Hessian heterogeneity, which struggle to directly explain this phenomenon. Towards bridging this gap in our understanding, by analyzing our Transformer training runs and simple quadratic settings inspired by the literature, we provide new insights, driven by stochastic differential equation models, into the role of batch size on the training dynamics.

SGD와 Adam의 트랜스포머 LM에 대한 학습 성능 차이의 원인에 대한 분석. SGD가 배치 크기가 커졌을 때의 수렴이 느리기 때문이라고 하네요. 원인으로는 그래디언트 노이즈에 대한 SGD와 Adam의 거동의 차이가 아닐까 추측하는군요.

<english>
Analysis on the reason of training gaps in transformer LM between SGD and Adam. It is because of convergence rate of SGD is slow when batch size became large. They suspect the reason of this is due to behavioral difference of SGD and Adam with respect to gradient noises.
</english>

#optimization #transformer 