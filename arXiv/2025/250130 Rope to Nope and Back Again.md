https://arxiv.org/abs/2501.18795

*Rope to Nope and Back Again: A New Hybrid Attention Strategy* (Bowen Yang, Bharat Venkitesh, Dwarak Talupuru, Hangyu Lin, David Cairuz, Phil Blunsom, Acyr Locatelli)

> Long-context large language models (LLMs) have achieved remarkable advancements, driven by techniques like Rotary Position Embedding (RoPE) (Su et al., 2023) and its extensions (Chen et al., 2023; Liu et al., 2024c; Peng et al., 2023). By adjusting RoPE parameters and incorporating training data with extended contexts, we can train performant models with considerably longer input sequences. However, existing RoPE-based methods exhibit performance limitations when applied to extended context lengths. This paper presents a comprehensive analysis of various attention mechanisms, including RoPE, No Positional Embedding (NoPE), and Query-Key Normalization (QK-Norm), identifying their strengths and shortcomings in long-context modeling. Our investigation identifies distinctive attention patterns in these methods and highlights their impact on long-context performance, providing valuable insights for architectural design. Building on these findings, we propose a novel architectural based on a hybrid attention mechanism that not only surpasses conventional RoPE-based transformer models in long context tasks but also achieves competitive performance on benchmarks requiring shorter context lengths.

RoPE, NoPE, 그리고 QK Norm의 Long Context 특성에 대한 분석. QK Norm이 Attention의 엔트로피를 높인다는 문제를 지적하고 있네요.

<english>
Analysis on characteristics of RoPE, NoPE, and QK norm in long context problems. They suggests QK norm increases entropy of attention.
</english>

#long-context #positional-encoding 