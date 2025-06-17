https://arxiv.org/abs/2505.22618

*Fast-dLLM: Training-free Acceleration of Diffusion LLM by Enabling KV Cache and Parallel Decoding* (Chengyue Wu, Hao Zhang, Shuchen Xue, Zhijian Liu, Shizhe Diao, Ligeng Zhu, Ping Luo, Song Han, Enze Xie)

> Diffusion-based large language models (Diffusion LLMs) have shown promise for non-autoregressive text generation with parallel decoding capabilities. However, the practical inference speed of open-sourced Diffusion LLMs often lags behind autoregressive models due to the lack of Key-Value (KV) Cache and quality degradation when decoding multiple tokens simultaneously. To bridge this gap, we introduce a novel block-wise approximate KV Cache mechanism tailored for bidirectional diffusion models, enabling cache reuse with negligible performance drop. Additionally, we identify the root cause of generation quality degradation in parallel decoding as the disruption of token dependencies under the conditional independence assumption. To address this, we propose a confidence-aware parallel decoding strategy that selectively decodes tokens exceeding a confidence threshold, mitigating dependency violations and maintaining generation quality. Experimental results on LLaDA and Dream models across multiple LLM benchmarks demonstrate up to \textbf{27.6$\times$ throughput} improvement with minimal accuracy loss, closing the performance gap with autoregressive models and paving the way for practical deployment of Diffusion LLMs.

Diffusion LM에 대해 KV 캐시를 도입한 연구가 하나 더 나왔군요. 이전 연구와 비슷하게 KV 캐시가 크게 변화하지 않는다는 것을 기반으로 했네요 (https://arxiv.org/abs/2505.15781). Diffusion LM에 대해 벌써 KV 캐시 연구까지 나왔다는 게 재미있습니다.

<english>
Additional attempt to introducing KV cache into diffusion LM. Similar to previous study, it is based on the observation that KV cache does not change much (https://arxiv.org/abs/2505.15781). I found it interesting that KV cache studies on diffusion LM appears already.
</english>

#diffusion #llm 