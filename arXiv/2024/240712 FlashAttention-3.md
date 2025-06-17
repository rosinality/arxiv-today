https://tridao.me/publications/flash3/flash3.pdf

*FlashAttention-3: Fast and Accurate Attention with Asynchrony and Low-precision* (Jay Shah, Ganesh Bikshandi, Ying Zhang, Vijay Thakkar, Pradeep Ramani, and Tri Dao)

> Attention, as a core layer of the ubiquitous Transformer architecture, is the bottleneck for large language models and long-context applications. FlashAttention elaborated an approach to speed up attention on GPUs through minimizing memory reads/writes. However, it has yet to take advantage of new capabilities present in recent hardware, with FlashAttention-2 achieving only 35% utilization on the H100 GPU. We develop three main techniques to speed up attention on Hopper GPUs: exploiting asynchrony of the Tensor Cores and TMA to (1) overlap overall computation and data movement via warp-specialization and (2) interleave block-wise matmul and softmax operations, and (3) block quantization and incoherent processing that leverages hardware support for FP8 low-precision. We demonstrate that our method, FlashAttention-3, achieves speedup on H100 GPUs by 1.5-2.0 with FP16 reaching up to 740 TFLOPs/s (75% utilization), and with FP8 reaching close to 1.2 PFLOPs/s. We validate that FP8 FlashAttention-3 achieves 2.6 lower numerical error than a baseline FP8 attention.

FlashAttention 3가 나왔군요. H100에서 FP16으로 75% Util을 달성했습니다. FP8은 여기에서 1.6배인 1.2 PFLOPS가 나오네요.

WGMMA와 TMA가 핵심인데 ThunderKittens (https://hazyresearch.stanford.edu/blog/2024-05-12-tk) 에서 저자들이 고통받았던 바로 그 오퍼레이션들이군요. 물론 Hopper 전용이긴 합니다.

#efficiency 