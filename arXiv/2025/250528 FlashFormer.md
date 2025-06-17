https://arxiv.org/abs/2505.22758

*FlashFormer: Whole-Model Kernels for Efficient Low-Batch Inference* (Aniruddha Nrusimha, William Brandon, Mayank Mishra, Yikang Shen, Rameswar Panda, Jonathan Ragan-Kelley, Yoon Kim)

> The size and compute characteristics of modern large language models have led to an increased interest in developing specialized kernels tailored for training and inference. Existing kernels primarily optimize for compute utilization, targeting the large-batch training and inference settings. However, low-batch inference, where memory bandwidth and kernel launch overheads contribute are significant factors, remains important for many applications of interest such as in edge deployment and latency-sensitive applications. This paper describes FlashFormer, a proof-of-concept kernel for accelerating single-batch inference for transformer-based large language models. Across various model sizes and quantizations settings, we observe nontrivial speedups compared to existing state-of-the-art inference kernels.

요즘 모델 전체를 하나의 커널로 만드는 시도들이 등장하네요 (https://hazyresearch.stanford.edu/blog/2025-05-27-no-bubbles).

<english>
Recently attempt to make a single kernel for entire model appears.
</english>

#efficiency 