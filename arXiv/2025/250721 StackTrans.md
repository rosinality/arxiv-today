https://arxiv.org/abs/2507.15343

*StackTrans: From Large Language Model to Large Pushdown Automata Model* (Kechi Zhang, Ge Li, Jia Li, Huangzhao Zhang, Yihong Dong, Jia Li, Jingjing Xu, Zhi Jin)

> The Transformer architecture has emerged as a landmark advancement within the broad field of artificial intelligence, effectively catalyzing the advent of large language models (LLMs). However, despite its remarkable capabilities and the substantial progress it has facilitated, the Transformer architecture still has some limitations. One such intrinsic limitation is its inability to effectively capture the Chomsky hierarchy, such as regular expressions or deterministic context-free grammars. Drawing inspiration from pushdown automata, which efficiently resolve deterministic context-free grammars using stacks, we propose StackTrans to address the aforementioned issue within LLMs. Unlike previous approaches that modify the attention computation, StackTrans explicitly incorporates hidden state stacks between Transformer layers. This design maintains compatibility with existing frameworks like flash-attention. Specifically, our design features stack operations -- such as pushing and popping hidden states -- that are differentiable and can be learned in an end-to-end manner. Our comprehensive evaluation spans benchmarks for both Chomsky hierarchies and large-scale natural languages. Across these diverse tasks, StackTrans consistently outperforms standard Transformer models and other baselines. We have successfully scaled StackTrans up from 360M to 7B parameters. In particular, our from-scratch pretrained model StackTrans-360M outperforms several larger open-source LLMs with 2-3x more parameters, showcasing its superior efficiency and reasoning capability.

Attention을 스택으로 교체.

Replacing attention with stacks.

#transformer #state-space-model 