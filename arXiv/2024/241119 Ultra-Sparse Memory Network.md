https://arxiv.org/abs/2411.12364

*Ultra-Sparse Memory Network* (Zihao Huang, Qiyang Min, Hongzhi Huang, Defa Zhu, Yutao Zeng, Ran Guo, Xun Zhou)

> It is widely acknowledged that the performance of Transformer models is exponentially related to their number of parameters and computational complexity. While approaches like Mixture of Experts (MoE) decouple parameter count from computational complexity, they still face challenges in inference due to high memory access costs. This work introduces UltraMem, incorporating large-scale, ultra-sparse memory layer to address these limitations. Our approach significantly reduces inference latency while maintaining model performance. We also investigate the scaling laws of this new architecture, demonstrating that it not only exhibits favorable scaling properties but outperforms traditional models. In our experiments, we train networks with up to 20 million memory slots. The results show that our method achieves state-of-the-art inference speed and model performance within a given computational budget.

Product Key Memory를 가져왔네요. (https://arxiv.org/abs/1907.05242) 여러 개선들을 붙이고 Tensor Decomposition과 Linear Projection을 통한 메모리 증폭을 결합했군요. 최근에도 Product Key Memory를 사용해보려는 시도가 있었죠. (https://arxiv.org/abs/2407.04153)

<english>
Sparse layer based on product key memory. (https://arxiv.org/abs/1907.05242) Incorporated various improvements and applied tensor decomposition and memory expansion using linear projection. There was recent study that also tried utilizing product key memory. (https://arxiv.org/abs/2407.04153)
</english>

#moe #transformer

# Links

[[200129 Product Key Memory.md]]