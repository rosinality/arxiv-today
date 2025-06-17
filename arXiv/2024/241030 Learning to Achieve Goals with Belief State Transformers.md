https://arxiv.org/abs/2410.23506

*Learning to Achieve Goals with Belief State Transformers* (Edward S. Hu, Kwangjun Ahn, Qinghua Liu, Haoran Xu, Manan Tomar, Ada Langford, Dinesh Jayaraman, Alex Lamb, John Langford)

> We introduce the "Belief State Transformer", a next-token predictor that takes both a prefix and suffix as inputs, with a novel objective of predicting both the next token for the prefix and the previous token for the suffix. The Belief State Transformer effectively learns to solve challenging problems that conventional forward-only transformers struggle with, in a domain-independent fashion. Key to this success is learning a compact belief state that captures all relevant information necessary for accurate predictions. Empirical ablations show that each component of the model is essential in difficult scenarios where standard Transformers fall short. For the task of story writing with known prefixes and suffixes, our approach outperforms the Fill-in-the-Middle method for reaching known goals and demonstrates improved performance even when the goals are unknown. Altogether, the Belief State Transformer enables more efficient goal-conditioned decoding, better test-time inference, and high-quality text representations on small scale problems.

Prefix와 Suffix의 조합에 대해 다음 토큰과 이전 토큰을 예측하는 Objective. FIM과 비슷하게 생각할 수 있지만 하나의 시퀀스에서 더 많은 학습 시그널을 추출한다고 생각할 수 있겠네요.

<english>
Training objective that predicts next and previous tokens for combinations of prefixes and suffixes. It maybe thought as similar objective to FIM, but it can may extract more training signal from a sequence.
</english>

#transformer 