https://arxiv.org/abs/2502.17416

*Reasoning with Latent Thoughts: On the Power of Looped Transformers* (Nikunj Saunshi, Nishanth Dikkala, Zhiyuan Li, Sanjiv Kumar, Sashank J. Reddi)

> Large language models have shown remarkable reasoning abilities and scaling laws suggest that large parameter count, especially along the depth axis, is the primary driver. In this work, we make a stronger claim -- many reasoning problems require a large depth but not necessarily many parameters. This unlocks a novel application of looped models for reasoning. Firstly, we show that for many synthetic reasoning problems like addition, $p$-hop induction, and math problems, a $k$-layer transformer looped $L$ times nearly matches the performance of a $kL$-layer non-looped model, and is significantly better than a $k$-layer model. This is further corroborated by theoretical results showing that many such reasoning problems can be solved via iterative algorithms, and thus, can be solved effectively using looped models with nearly optimal depth. Perhaps surprisingly, these benefits also translate to practical settings of language modeling -- on many downstream reasoning tasks, a language model with $k$-layers looped $L$ times can be competitive to, if not better than, a $kL$-layer language model. In fact, our empirical analysis reveals an intriguing phenomenon: looped and non-looped models exhibit scaling behavior that depends on their effective depth, akin to the inference-time scaling of chain-of-thought (CoT) reasoning. We further elucidate the connection to CoT reasoning by proving that looped models implicitly generate latent thoughts and can simulate $T$ steps of CoT with $T$ loops. Inspired by these findings, we also present an interesting dichotomy between reasoning and memorization, and design a looping-based regularization that is effective on both fronts.

Looped Transformer 연구가 또 나왔군요. Perplexity와는 별개로 추론 능력에서 강점이 있었다는 결과입니다. Weight가 유사하도록 Regularization을 걸어준 경우에도 비슷한 효과가 나타났다고 하네요.

Looped Transformer가 Continuous Thought라는 아이디어와 연관되어 등장하고 있죠. 일단 저는 Discrete Thought가 프리트레이닝에서 가이드를 더 크게 받을 수 있기에 유리하지 않을까 생각하긴 합니다. 그렇지만 늘 흥미로운 주제죠.

<english>
One more research on looped transformer. Beside of perplexity, the author says there were benefits for reasoning abilities. They also said similar effect occurs when they use regularization that making weights similar.

Looped transformers appears with the concept of continuous thoughts nowadays. I think discrete thought could be better because they can use information the model got during pretraining. But it is always intruiging idea.
</english>

#transformer #reasoning 