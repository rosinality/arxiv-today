https://arxiv.org/abs/2502.11089

*Native Sparse Attention: Hardware-Aligned and Natively Trainable Sparse Attention* (Jingyang Yuan, Huazuo Gao, Damai Dai, Junyu Luo, Liang Zhao, Zhengyan Zhang, Zhenda Xie, Y. X. Wei, Lean Wang, Zhiping Xiao, Yuqing Wang, Chong Ruan, Ming Zhang, Wenfeng Liang, Wangding Zeng)

> Long-context modeling is crucial for next-generation language models, yet the high computational cost of standard attention mechanisms poses significant computational challenges. Sparse attention offers a promising direction for improving efficiency while maintaining model capabilities. We present NSA, a Natively trainable Sparse Attention mechanism that integrates algorithmic innovations with hardware-aligned optimizations to achieve efficient long-context modeling. NSA employs a dynamic hierarchical sparse strategy, combining coarse-grained token compression with fine-grained token selection to preserve both global context awareness and local precision. Our approach advances sparse attention design with two key innovations: (1) We achieve substantial speedups through arithmetic intensity-balanced algorithm design, with implementation optimizations for modern hardware. (2) We enable end-to-end training, reducing pretraining computation without sacrificing model performance. As shown in Figure 1, experiments show the model pretrained with NSA maintains or exceeds Full Attention models across general benchmarks, long-context tasks, and instruction-based reasoning. Meanwhile, NSA achieves substantial speedups over Full Attention on 64k-length sequences across decoding, forward propagation, and backward propagation, validating its efficiency throughout the model lifecycle.

DeepSeek은 Sparse Attention을 태클하고 있었군요. Token Pooling, Top-K Block Selection, Sliding Window의 조합이네요. DeepSeek V3에서 미래에 Long Context 문제를 태클할 것이라고 했었는데 예상하지 못했던 방향이네요. Sparse Attention을 다시 생각해보는 것이 좋을지도 모르겠습니다. (https://arxiv.org/abs/2502.12082)

<english>
DeepSeek was tackling sparse attention. It is combindation of token pooling, top-K block selection, sliding window. They said they will investigate long context problems in the future in DeepSeek V3 paper, but it is not a direction I have expected. Maybe it is worth to consider sparse attention again (https://arxiv.org/abs/2502.12082). 
</english>

#sparsity #efficiency #efficient-training 