https://arxiv.org/abs/2412.19255

*Multi-matrix Factorization Attention* (Jingcheng Hu, Houyi Li, Yinmin Zhang, Zili Wang, Shuigeng Zhou, Xiangyu Zhang, Heung-Yeung Shum)

> We propose novel attention architectures, Multi-matrix Factorization Attention (MFA) and MFA-Key-Reuse (MFA-KR). Existing variants for standard Multi-Head Attention (MHA), including SOTA methods like MLA, fail to maintain as strong performance under stringent Key-Value cache (KV cache) constraints. MFA enhances model capacity by efficiently scaling up both the number and dimension of attention heads through low-rank matrix factorization in the Query-Key (QK) circuit. Extending MFA, MFA-KR further reduces memory requirements by repurposing the key cache as value through value projection re-parameterization. MFA's design enables strong model capacity when working under tight KV cache budget, while MFA-KR is suitable for even harsher KV cache limits with minor performance trade-off. Notably, in our extensive and large-scale experiments, the proposed architecture outperforms MLA and performs comparably to MHA, while reducing KV cache usage by up to 56% and 93.7%, respectively.

DeepSeek-V3 덕에 MLA에 대한 주목도 좀 더 늘어난 느낌이군요. MLA에서 Key/Value에 대한 Up projection 행렬을 합쳐놓은 형태네요.

<english>
Recently MLA is gaining popularity due to DeepSeek-V3. This method is similar to combining up projection matrices for key/value in MLA.
</english>

#attention #efficiency 