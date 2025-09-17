https://arxiv.org/abs/2509.05282

*Elucidating the Design Space of Decay in Linear Attention* (Zhen Qin, Xuyang Shen, Yiran Zhong)

> This paper presents a comprehensive investigation into the decay mechanisms inherent in linear complexity sequence models. We systematically delineate the design space of decay mechanisms across four pivotal dimensions: parameterization strategy, which refers to the computational methodology for decay; parameter sharing, which involves the utilization of supplementary parameters for decay computation; decay granularity, comparing scalar versus vector-based decay; and compatibility with relative positional encoding methods, such as Rotary Position Embedding (RoPE). Through an extensive series of experiments conducted on diverse language modeling tasks, we uncovered several critical insights. Firstly, the design of the parameterization strategy for decay requires meticulous consideration. Our findings indicate that effective configurations are typically confined to a specific range of parameters. Secondly, parameter sharing cannot be used arbitrarily, as it may cause decay values to be too large or too small, thereby significantly impacting performance. Thirdly, under identical parameterization strategies, scalar decay generally underperforms compared to its vector-based counterpart. However, in certain scenarios with alternative parameterization strategies, scalar decay may unexpectedly surpass vector decay in efficacy. Lastly, our analysis reveals that RoPE, a commonly employed relative positional encoding method, typically fails to provide tangible benefits to the majority of linear attention mechanisms.

State Space Model의 Decay 요인에 대한 비교 연구.

Comparison of decay factors of state-space models.

#state-space-model 