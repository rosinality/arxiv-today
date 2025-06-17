https://arxiv.org/abs/2410.20399

*ThunderKittens: Simple, Fast, and Adorable AI Kernels* (Benjamin F. Spector, Simran Arora, Aaryan Singhal, Daniel Y. Fu, Christopher Ré)

> The challenge of mapping AI architectures to GPU hardware is creating a critical bottleneck in AI progress. Despite substantial efforts, hand-written custom kernels fail to meet their theoretical performance thresholds, even on well-established operations like linear attention. The diverse hardware capabilities of GPUs might suggest that we need a wide variety of techniques to achieve high performance. However, our work explores whether a small number of key abstractions can drastically simplify the process. We present ThunderKittens (TK), a framework for writing performant AI kernels while remaining easy to use and maintain. Our abstractions map to the three levels of the GPU hierarchy: (1) at the warp-level, we provide 16x16 matrix tiles as basic data structures and PyTorch-like parallel compute operations over tiles, (2) at the thread-block level, we provide a template for overlapping asynchronous operations across parallel warps, and (3) at the grid-level, we provide support to help hide the block launch and tear-down, and memory costs. We show the value of TK by providing kernels that match or outperform prior kernels for a range of AI operations. We match CuBLAS and FlashAttention-3 on GEMM and attention inference performance and outperform the strongest baselines by $10-40\%$ on attention backwards, $8\times$ on state space models, and $14\times$ on linear attention.

ThunderKittens의 (https://hazyresearch.stanford.edu/blog/2024-05-12-tk) 논문이 나왔군요. 실제 써보면 느낌이 어떨지 궁금하네요.

<english>
Paper on ThunderKittens. (https://hazyresearch.stanford.edu/blog/2024-05-12-tk) I wonder how it will feel if I use in real situations.
</english>

#efficiency 