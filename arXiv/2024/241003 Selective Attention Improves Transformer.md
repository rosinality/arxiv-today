https://arxiv.org/abs/2410.02703

*Selective Attention Improves Transformer* (Yaniv Leviathan, Matan Kalman, Yossi Matias)

> Unneeded elements in the attention's context degrade performance. We introduce Selective Attention, a simple parameter-free change to the standard attention mechanism which reduces attention to unneeded elements. Selective attention improves language modeling performance in a variety of model sizes and context lengths. For example, a range of transformers trained with the language modeling objective on C4 with selective attention perform equivalently to standard transformers with ~2X more heads and parameters in their attention modules. Selective attention also allows decreasing the size of the attention's context buffer, leading to meaningful reductions in the memory and compute requirements during inference. For example, transformers with 100M parameters trained on C4 with context sizes of 512, 1,024, and 2,048 need 16X, 25X, and 47X less memory for their attention module, respectively, when equipped with selective attention, as those without selective attention, with the same validation perplexity.

Attention Logit에 대한 cumsum을 사용한 Positional Encoding. Contextual Position Encoding과 (https://arxiv.org/abs/2405.18719) 비슷한 느낌이 나네요.

효과가 나타나긴 하는데 가장 중요한 문제는 이를 효율적으로 계산할 수 있는 Attention 구현이 가능한가 하는 것이겠죠.

<english>
Positional encoding that using cumsum with attention logit. It seems similar to Contextual Position Encoding (https://arxiv.org/abs/2405.18719)

The result showed performance improvements but important problems is that we can make an implementation that be able to calculate this efficiently.
</english>

#positional-encoding

# Links

[[240529 Contextual Position Encoding.md]]