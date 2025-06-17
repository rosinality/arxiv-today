https://arxiv.org/abs/2503.07680

*Hierarchical Balance Packing: Towards Efficient Supervised Fine-tuning for Long-Context LLM* (Yongqiang Yao, Jingru Tan, Kaihuan Liang, Feizhao Zhang, Yazhe Niu, Jiahao Hu, Ruihao Gong, Dahua Lin, Ningyi Xu)

> Training Long-Context Large Language Models (LLMs) is challenging, as hybrid training with long-context and short-context data often leads to workload imbalances. Existing works mainly use data packing to alleviate this issue but fail to consider imbalanced attention computation and wasted communication overhead. This paper proposes Hierarchical Balance Packing (HBP), which designs a novel batch-construction method and training recipe to address those inefficiencies. In particular, the HBP constructs multi-level data packing groups, each optimized with a distinct packing length. It assigns training samples to their optimal groups and configures each group with the most effective settings, including sequential parallelism degree and gradient checkpointing configuration. To effectively utilize multi-level groups of data, we design a dynamic training pipeline specifically tailored to HBP, including curriculum learning, adaptive sequential parallelism, and stable loss. Our extensive experiments demonstrate that our method significantly reduces training time over multiple datasets and open-source models while maintaining strong performance. For the largest DeepSeek-V2 (236B) MOE model, our method speeds up the training by 2.4$\times$ with competitive performance.

Long Context 학습이 중요해지니 Packing 과정에서 굳이 짧은 시퀀스를 이어붙여서 Context Parallel이 필요하게 만들지 말자는 아이디어가 나오는군요. (https://arxiv.org/abs/2502.21231)

<english>
As long context training became important, the idea of we should not make context parallel is required by concatenating short sequences during packing process  (https://arxiv.org/abs/2502.21231).
</english>

#long-context #parallelism #efficiency 
