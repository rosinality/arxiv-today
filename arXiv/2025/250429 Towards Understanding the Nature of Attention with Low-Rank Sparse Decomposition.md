https://arxiv.org/abs/2504.20938

*Towards Understanding the Nature of Attention with Low-Rank Sparse Decomposition* (Zhengfu He, Junxuan Wang, Rui Lin, Xuyang Ge, Wentao Shu, Qiong Tang, Junping Zhang, Xipeng Qiu)

> We propose Low-Rank Sparse Attention (Lorsa), a sparse replacement model of Transformer attention layers to disentangle original Multi Head Self Attention (MHSA) into individually comprehensible components. Lorsa is designed to address the challenge of attention superposition to understand attention-mediated interaction between features in different token positions. We show that Lorsa heads find cleaner and finer-grained versions of previously discovered MHSA behaviors like induction heads, successor heads and attention sink behavior (i.e., heavily attending to the first token). Lorsa and Sparse Autoencoder (SAE) are both sparse dictionary learning methods applied to different Transformer components, and lead to consistent findings in many ways. For instance, we discover a comprehensive family of arithmetic-specific Lorsa heads, each corresponding to an atomic operation in Llama-3.1-8B. Automated interpretability analysis indicates that Lorsa achieves parity with SAE in interpretability while Lorsa exhibits superior circuit discovery properties, especially for features computed collectively by multiple MHSA heads. We also conduct extensive experiments on architectural design ablation, Lorsa scaling law and error analysis.

SAE처럼 Attention의 Monosemantic Feature를 추출하기 위한 방법. Value의 차원을 1로 줄이고 헤드를 늘린 다음 Top K 헤드를 선택하는 방법이군요.

<english>
A method of extracting monosemantic feature from attention, like SAE. The method is reduce dimension of value into 1 and increases number of heads, then choose top K heads.
</english>

#mechanistic-interpretation 