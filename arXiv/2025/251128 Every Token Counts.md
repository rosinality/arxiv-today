https://arxiv.org/abs/2511.23319

*Every Token Counts: Generalizing 16M Ultra-Long Context in Large Language Models* (Xiang Hu, Zhanchao Zhou, Ruiqi Liang, Zehuan Li, Wei Wu, Jianguo Li)

> This work explores the challenge of building ``Machines that Can Remember'', framing long-term memory as the problem of efficient ultra-long context modeling. We argue that this requires three key properties: \textbf{sparsity}, \textbf{random-access flexibility}, and \textbf{length generalization}. To address ultra-long-context modeling, we leverage Hierarchical Sparse Attention (HSA), a novel attention mechanism that satisfies all three properties. We integrate HSA into Transformers to build HSA-UltraLong, which is an 8B-parameter MoE model trained on over 8 trillion tokens and is rigorously evaluated on different tasks with in-domain and out-of-domain context lengths to demonstrate its capability in handling ultra-long contexts. Results show that our model performs comparably to full-attention baselines on in-domain lengths while achieving over 90\% accuracy on most in-context retrieval tasks with contexts up to 16M. This report outlines our experimental insights and open problems, contributing a foundation for future research in ultra-long context modeling.

새로운 Sparse Attention 디자인. 1. top-K Retrieval과 Attention 계산에 다른 쿼리를 사용 2. 각 청크에 대한 Attention은 청크를 모두 합쳐서 계산하는 대신 각 청크에 대해 계산한 다음 가중합을 취함.

Novel design of sparse attention. 1. This uses separate queries for top-K retrieval and attention computation. 2. Attention is computed on each chunk separately and weighted sum is done over chunks, instead of concatenating all of the chunks.

#sparse-attention #efficiency #sparsity 