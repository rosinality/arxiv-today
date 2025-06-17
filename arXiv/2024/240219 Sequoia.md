https://arxiv.org/abs/2402.12374

*Sequoia: Scalable, Robust, and Hardware-aware Speculative Decoding* (Zhuoming Chen, Avner May, Ruslan Svirschevski, Yuhsun Huang, Max Ryabinin, Zhihao Jia, Beidi Chen)

> As the usage of large language models (LLMs) grows, performing efficient inference with these models becomes increasingly important. While speculative decoding has recently emerged as a promising direction for speeding up inference, existing methods are limited in their ability to scale to larger speculation budgets, and adapt to different hyperparameters and hardware. This paper introduces Sequoia, a scalable, robust, and hardware-aware algorithm for speculative decoding. To attain better scalability, Sequoia introduces a dynamic programming algorithm to find the optimal tree structure for the speculated tokens. To achieve robust speculative performance, Sequoia uses a novel sampling and verification method that outperforms prior work across different decoding temperatures. Finally, Sequoia introduces a hardware-aware tree optimizer that maximizes speculative performance by automatically selecting the token tree size and depth for a given hardware platform. Evaluation shows that Sequoia improves the decoding speed of Llama2-7B, Llama2-13B, and Vicuna-33B on an A100 by up to $4.04\times$, $3.84\times$, and $2.37\times$, and Llama2-70B offloading by up to $10.33\times$ on L40.

Speculative Decoding에서 후보 시퀀스를 하나 뽑는 것이 아니라 토큰들의 트리를 구성하는 방법. 여기서 Top-K 토큰으로 확장하는 것이 아니라 Verification을 통과할 토큰을 최대화하는 방식으로 트리를 구성한다는 것이 주 아이디어입니다.

#efficiency 