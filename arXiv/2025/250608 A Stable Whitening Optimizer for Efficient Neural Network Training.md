https://arxiv.org/abs/2506.07254

*A Stable Whitening Optimizer for Efficient Neural Network Training* (Kevin Frans, Sergey Levine, Pieter Abbeel)

> In this work, we take an experimentally grounded look at neural network optimization. Building on the Shampoo family of algorithms, we identify and alleviate three key issues, resulting in the proposed SPlus method. First, we find that naive Shampoo is prone to divergence when matrix-inverses are cached for long periods. We introduce an alternate bounded update combining a historical eigenbasis with instantaneous normalization, resulting in across-the-board stability and significantly lower computational requirements. Second, we adapt a shape-aware scaling to enable learning rate transfer across network width. Third, we find that high learning rates result in large parameter noise, and propose a simple iterate-averaging scheme which unblocks faster learning. To properly confirm these findings, we introduce a pointed Transformer training benchmark, considering three objectives (language modelling, image classification, and diffusion modelling) across different stages of training. On average, SPlus is able to reach the validation performance of Adam within 44% of the gradient steps and 62% of the wallclock time.

Shampoo의 개선. Shampoo를 안정화시키고 Hyperparameter Transfer, 그리고 EMA를 추가했네요. EMA가 추가되어서 비교가 어렵긴 하군요.

<english>
An improvement of Shampoo. First stabilizes Shampoo, and adds hyperparameter transfer and EMA. As EMA is introduced fair comparison is somewhat harder.
</english>

#optimizer 