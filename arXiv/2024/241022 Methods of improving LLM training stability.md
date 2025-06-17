https://arxiv.org/abs/2410.16682

*Methods of improving LLM training stability* (Oleg Rybakov, Mike Chrzanowski, Peter Dykas, Jinze Xue, Ben Lanir)

> Training stability of large language models(LLMs) is an important research topic. Reproducing training instabilities can be costly, so we use a small language model with 830M parameters and experiment with higher learning rates to force models to diverge. One of the sources of training instability is the growth of logits in attention layers. We extend the focus of the previous work and look not only at the magnitude of the logits but at all outputs of linear layers in the Transformer block. We observe that with a high learning rate the L2 norm of all linear layer outputs can grow with each training step and the model diverges. Specifically we observe that QKV, Proj and FC2 layers have the largest growth of the output magnitude. This prompts us to explore several options: 1) apply layer normalization not only after QK layers but also after Proj and FC2 layers too; 2) apply layer normalization after the QKV layer (and remove pre normalization). 3) apply QK layer normalization together with softmax capping. We show that with the last two methods we can increase learning rate by 1.5x (without model divergence) in comparison to an approach based on QK layer normalization only. Also we observe significant perplexity improvements for all three methods in comparison to the baseline model.

QK Norm 같은 트랜스포머 학습 안정성을 위한 테크닉들을 실험해봤군요. 저는 Softcapping과 Post Norm의 조합이 꽤 괜찮다고 생각합니다. 다만 이 조합은 실험에는 없네요.

<english>
Experiments on training stability techniques for transformers like QK Norm. I think combination of softcapping and post norm is good. But this combination does not tried in the paper.
</english>

#transformer 