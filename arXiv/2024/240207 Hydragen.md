https://arxiv.org/abs/2402.05099

*Hydragen: High-Throughput LLM Inference with Shared Prefixes* (Jordan Juravsky, Bradley Brown, Ryan Ehrlich, Daniel Y. Fu, Christopher Ré, Azalia Mirhoseini)

> Transformer-based large language models (LLMs) are now deployed to hundreds of millions of users. LLM inference is commonly performed on batches of sequences that share a prefix, such as few-shot examples or a chatbot system prompt. Decoding in this large-batch setting can be bottlenecked by the attention operation, which reads large key-value (KV) caches from memory and computes inefficient matrix-vector products for every sequence in the batch. In this work, we introduce Hydragen, a hardware-aware exact implementation of attention with shared prefixes. Hydragen computes attention over the shared prefix and unique suffixes separately. This decomposition enables efficient prefix attention by batching queries together across sequences, reducing redundant memory reads and enabling the use of hardware-friendly matrix multiplications. Our method can improve end-to-end LLM throughput by up to 32x against competitive baselines, with speedup growing with the batch size and shared prefix length. Hydragen also enables the use of very long shared contexts: with a high batch size, increasing the prefix length from 1K to 16K tokens decreases Hydragen throughput by less than 15%, while the throughput of baselines drops by over 90%. Hydragen generalizes beyond simple prefix-suffix decomposition and can be applied to tree-based prompt sharing patterns, allowing us to further reduce inference time on competitive programming problems by 55%.

Prefix, 즉 입력의 앞 부분을 공유하는 경우에 대해서 LLM 추론 속도를 향상시키기 위한 방법. vLLM이나 Radix Attention의 최적화에 더해 Attention 계산 자체에서 중복을 제거하는 것을 목표로 합니다.

#efficiency 

Improving inference performance of LLMs when prefix, that is, front part of input is shared. On the top of optimizations of vLLM and Radix Attention this approach removes duplications in attention computation.