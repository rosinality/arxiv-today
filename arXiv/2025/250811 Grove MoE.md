https://arxiv.org/abs/2508.07785

*Grove MoE: Towards Efficient and Superior MoE LLMs with Adjugate Experts* (Haoyuan Wu, Haoxing Chen, Xiaodong Chen, Zhanchao Zhou, Tieyuan Chen, Yihong Zhuang, Guoshan Lu, Zenan Huang, Junbo Zhao, Lin Liu, Zhenzhong Lan, Bei Yu, Jianguo Li)

> The Mixture of Experts (MoE) architecture is a cornerstone of modern state-of-the-art (SOTA) large language models (LLMs). MoE models facilitate scalability by enabling sparse parameter activation. However, traditional MoE architecture uses homogeneous experts of a uniform size, activating a fixed number of parameters irrespective of input complexity and thus limiting computational efficiency. To overcome this limitation, we introduce Grove MoE, a novel architecture incorporating experts of varying sizes, inspired by the heterogeneous big.LITTLE CPU architecture. This architecture features novel adjugate experts with a dynamic activation mechanism, enabling model capacity expansion while maintaining manageable computational overhead. Building on this architecture, we present GroveMoE-Base and GroveMoE-Inst, 33B-parameter LLMs developed by applying an upcycling strategy to the Qwen3-30B-A3B-Base model during mid-training and post-training. GroveMoE models dynamically activate 3.14-3.28B parameters based on token complexity and achieve performance comparable to SOTA open-source models of similar or even larger size.

Sparse Upcycling 개선. 여기서는 MoE 모델을 가져와 다시 한 번 확장하는 형태. Expert들을 그룹으로 나누고 각 그룹에 Adjoint Expert를 부여해서 각 그룹 내의 Expert의 출력에 더해주는 방법. Shared Expert의 그룹 버전?

Improvement on sparse upcycling. They take an existing MoE model and expand it further. The method is dividing experts into groups and assigning an adjugate expert to each group, which adds its output to the outputs of the experts within each group. This can be a group version of shared experts.

#moe 