https://arxiv.org/abs/2411.12992

*MemoryFormer: Minimize Transformer Computation by Removing Fully-Connected Layers* (Ning Ding, Yehui Tang, Haochen Qin, Zhenli Zhou, Chao Xu, Lin Li, Kai Han, Heng Liao, Yunhe Wang)

> In order to reduce the computational complexity of large language models, great efforts have been made to to improve the efficiency of transformer models such as linear attention and flash-attention. However, the model size and corresponding computational complexity are constantly scaled up in pursuit of higher performance. In this work, we present MemoryFormer, a novel transformer architecture which significantly reduces the computational complexity (FLOPs) from a new perspective. We eliminate nearly all the computations of the transformer model except for the necessary computation required by the multi-head attention operation. This is made possible by utilizing an alternative method for feature transformation to replace the linear projection of fully-connected layers. Specifically, we first construct a group of in-memory lookup tables that store a large amount of discrete vectors to replace the weight matrix used in linear projection. We then use a hash algorithm to retrieve a correlated subset of vectors dynamically based on the input embedding. The retrieved vectors combined together will form the output embedding, which provides an estimation of the result of matrix multiplication operation in a fully-connected layer. Compared to conducting matrix multiplication, retrieving data blocks from memory is a much cheaper operation which requires little computations. We train MemoryFormer from scratch and conduct extensive experiments on various benchmarks to demonstrate the effectiveness of the proposed model.

이진 코드 기반 해시 테이블로 FFN을 대체. Finite Scalar Quantization으로 FFN을 대체했다는 느낌이군요. Product Key Memory도 그렇고 요즘 이런 시도를 많이 하네요.

<english>
Replacing FFN with hash table based on binary codes. It can be thought as replacing FFN with finite scalar quantization. Aside of product key memory, there are many similar approaches appearing nowadays.
</english>

#transformer 