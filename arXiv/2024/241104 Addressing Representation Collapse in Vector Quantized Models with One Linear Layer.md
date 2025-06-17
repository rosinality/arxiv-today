https://arxiv.org/abs/2411.02038

*Addressing Representation Collapse in Vector Quantized Models with One Linear Layer* (Yongxin Zhu, Bocheng Li, Yifei Xin, Linli Xu)

> Vector Quantization (VQ) is a widely used method for converting continuous representations into discrete codes, which has become fundamental in unsupervised representation learning and latent generative models. However, VQ models are often hindered by the problem of representation collapse in the latent space, which leads to low codebook utilization and limits the scalability of the codebook for large-scale training. Existing methods designed to mitigate representation collapse typically reduce the dimensionality of latent space at the expense of model capacity, which do not fully resolve the core issue. In this study, we conduct a theoretical analysis of representation collapse in VQ models and identify its primary cause as the disjoint optimization of the codebook, where only a small subset of code vectors are updated through gradient descent. To address this issue, we propose \textbf{SimVQ}, a novel method which reparameterizes the code vectors through a linear transformation layer based on a learnable latent basis. This transformation optimizes the \textit{entire linear space} spanned by the codebook, rather than merely updating \textit{the code vector} selected by the nearest-neighbor search in vanilla VQ models. Although it is commonly understood that the multiplication of two linear matrices is equivalent to applying a single linear layer, our approach works surprisingly well in resolving the collapse issue in VQ models with just one linear layer. We validate the efficacy of SimVQ through extensive experiments across various modalities, including image and audio data with different model architectures. Our code is available at \url{https://github.com/youngsheen/SimVQ}.

VQ 학습의 문제가 코드북의 일부만 업데이트 되는 것에 있다는 아이디어. 해결 방법은 코드북 C만 학습하는 것이 아니라 새로운 행렬 W를 도입해서 CW를 학습하는 것입니다. 단순하면서도 강력하군요.

<english>
Problem of training VQ model is due to only partial entries in codebook are updated. Resolution for this is that not only learn codebook C, instead they used new parameterization that by introducing new matrix W, and learn CW. Simple but powerful.
</english>

#vq 