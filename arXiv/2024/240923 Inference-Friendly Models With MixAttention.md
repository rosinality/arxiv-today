https://arxiv.org/abs/2409.15012

*Inference-Friendly Models With MixAttention* (Shashank Rajput, Ying Sheng, Sean Owen, Vitaliy Chiley)

> The size of the key-value (KV) cache plays a critical role in determining both the maximum context length and the number of concurrent requests supported during inference in modern language models. The KV cache size grows proportionally with the number of attention heads and the tokens processed, leading to increased memory consumption and slower inference for long inputs. In this work, we explore the use of MixAttention, a model architecture modification closely related to a blog published by Character.AI. MixAttention combines sliding window attention, where only a small subset of recent tokens is stored in the KV cache, with KV cache sharing across layers. Our experiments demonstrate that MixAttention significantly reduces memory usage and improves inference speed without sacrificing model performance in both short and long-context tasks. We also explore various configurations of this architecture, identifying those that maintain quality across evaluation metrics while optimizing resource efficiency.

