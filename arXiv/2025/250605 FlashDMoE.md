https://arxiv.org/abs/2506.04667

*FlashDMoE: Fast Distributed MoE in a Single Kernel* (Osayamen Jonathan Aimuyo, Byungsoo Oh, Rachee Singh)

> The computational sparsity of Mixture-of-Experts (MoE) models enables sub-linear growth in compute cost as model size increases, offering a scalable path to training massive neural networks. However, existing implementations suffer from \emph{low GPU utilization}, \emph{significant latency overhead}, and a fundamental \emph{inability to leverage task locality}, primarily due to CPU-managed scheduling, host-initiated communication, and frequent kernel launches. To overcome these limitations, we develop FlashDMoE, a fully GPU-resident MoE operator that fuses expert computation and inter-GPU communication into a \emph{single persistent GPU kernel}. FlashDMoE enables fine-grained pipelining of dispatch, compute, and combine phases, eliminating launch overheads and reducing idle gaps. Its device-initiated communication protocol introduces \emph{payload-efficient} data transfers, significantly shrinking buffer sizes in sparsely activated MoE layers. When evaluated on a single 8-H100 GPU node with MoE models having up to 128 experts and 16K token sequences, FlashDMoE achieves up to \textbf{6}x lower latency, \textbf{5,7}x higher throughput, \textbf{4}x better weak scaling efficiency, and \textbf{9}x higher GPU utilization compared to state-of-the-art baselines, despite using FP32 while baselines use FP16. FlashDMoE demonstrates that principled GPU kernel-hardware co-design is key to unlocking the performance ceiling of large-scale distributed ML workloads.

MoE를 위한 단일 커널. 다만 현재 FP32에 대해서만 구현됐군요.

<english>
Fused single kernel for MoE. But currently only implemented for FP32.
</english>

#moe #efficiency 