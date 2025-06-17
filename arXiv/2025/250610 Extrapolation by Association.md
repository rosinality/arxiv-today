https://arxiv.org/abs/2506.09251

*Extrapolation by Association: Length Generalization Transfer in Transformers* (Ziyang Cai, Nayoung Lee, Avi Schwarzschild, Samet Oymak, Dimitris Papailiopoulos)

> Transformer language models have demonstrated impressive generalization capabilities in natural language domains, yet we lack a fine-grained understanding of how such generalization arises. In this paper, we investigate length generalization--the ability to extrapolate from shorter to longer inputs--through the lens of \textit{task association}. We find that length generalization can be \textit{transferred} across related tasks. That is, training a model with a longer and related auxiliary task can lead it to generalize to unseen and longer inputs from some other target task. We demonstrate this length generalization transfer across diverse algorithmic tasks, including arithmetic operations, string transformations, and maze navigation. Our results show that transformer models can inherit generalization capabilities from similar tasks when trained jointly. Moreover, we observe similar transfer effects in pretrained language models, suggesting that pretraining equips models with reusable computational scaffolding that facilitates extrapolation in downstream settings. Finally, we provide initial mechanistic evidence that length generalization transfer correlates with the re-use of the same attention heads between the tasks. Together, our findings deepen our understanding of how transformers generalize to out-of-distribution inputs and highlight the compositional reuse of inductive structure across tasks.

Long Context 과제를 사용해서 학습하면 Short Context로만 학습한 과제도 Length Generalization이 일어날 수 있다는 분석. Long Context 학습을 할 때 기대하는 현상이긴 하죠.

<english>
An analysis suggest that length generalization for the tasks only trained with short contexts can happen if it is also trained with long context tasks. It is what expected when long context training.
</english>

#transformer #long-context 