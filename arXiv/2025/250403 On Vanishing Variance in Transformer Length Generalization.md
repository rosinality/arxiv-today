https://arxiv.org/abs/2504.02827

*On Vanishing Variance in Transformer Length Generalization* (Ruining Li, Gabrijel Boduljak, Jensen (Jinghao)Zhou)

> It is a widely known issue that Transformers, when trained on shorter sequences, fail to generalize robustly to longer ones at test time. This raises the question of whether Transformer models are real reasoning engines, despite their impressive abilities in mathematical problem solving and code synthesis. In this paper, we offer a vanishing variance perspective on this issue. To the best of our knowledge, we are the first to demonstrate that even for today's frontier models, a longer sequence length results in a decrease in variance in the output of the multi-head attention modules. On the argmax retrieval and dictionary lookup tasks, our experiments show that applying layer normalization after the attention outputs leads to significantly better length generalization. Our analyses attribute this improvement to a reduction-though not a complete elimination-of the distribution shift caused by vanishing variance.

Long Context 상황에서 Attention 출력의 분산이 낮아지는 것이 문제라는 지적. Attention Score의 엔트로피가 높아지는 것과 연결해서 생각할 수 있을 것 같네요. 완화하는 방법은 Attention 출력에 Layer Norm을 붙이는 것이라고. Post Norm이군요.

<english>
The author pointed out reduction of variance of attention output in long context situation is problematic. I think it can be linked with the problem of increase of entropy of attention scores. They relieved ith by using layer norm after attention outputs. It's post norm.
</english>

#transformer #long-context 