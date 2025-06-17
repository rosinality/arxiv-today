https://arxiv.org/abs/2505.15431

*Hunyuan-TurboS: Advancing Large Language Models through Mamba-Transformer Synergy and Adaptive Chain-of-Thought* (Tencent Hunyuan Team)

> As Large Language Models (LLMs) rapidly advance, we introduce Hunyuan-TurboS, a novel large hybrid Transformer-Mamba Mixture of Experts (MoE) model. It synergistically combines Mamba's long-sequence processing efficiency with Transformer's superior contextual understanding. Hunyuan-TurboS features an adaptive long-short chain-of-thought (CoT) mechanism, dynamically switching between rapid responses for simple queries and deep "thinking" modes for complex problems, optimizing computational resources. Architecturally, this 56B activated (560B total) parameter model employs 128 layers (Mamba2, Attention, FFN) with an innovative AMF/MF block pattern. Faster Mamba2 ensures linear complexity, Grouped-Query Attention minimizes KV cache, and FFNs use an MoE structure. Pre-trained on 16T high-quality tokens, it supports a 256K context length and is the first industry-deployed large-scale Mamba model. Our comprehensive post-training strategy enhances capabilities via Supervised Fine-Tuning (3M instructions), a novel Adaptive Long-short CoT Fusion method, Multi-round Deliberation Learning for iterative improvement, and a two-stage Large-scale Reinforcement Learning process targeting STEM and general instruction-following. Evaluations show strong performance: overall top 7 rank on LMSYS Chatbot Arena with a score of 1356, outperforming leading models like Gemini-2.0-Flash-001 (1352) and o4-mini-2025-04-16 (1345). TurboS also achieves an average of 77.9% across 23 automated benchmarks. Hunyuan-TurboS balances high performance and efficiency, offering substantial capabilities at lower inference costs than many reasoning models, establishing a new paradigm for efficient large-scale pre-trained models.

텐센트 LLM. Mamba2 하이브리드. 정답 기반 Generative RM을 사용. 헤드 결합 하이브리드 모델도 이번에 나왔던데 (https://falcon-lm.github.io/blog/falcon-h1/) 이미 다들 하이브리드 혹은 Sparse Attention으로 넘어가고 있는 것이 아닌가 싶네요.

<english>
Tencent's LLM. It's Mamba2 hybrid. Used generative RM with reference answers. There was head combined hybrid model appeared recently (https://falcon-lm.github.io/blog/falcon-h1/) maybe everyone are going to hybrid or sparse attentions.
</english>

#llm #state-space-model #reasoning #rl 