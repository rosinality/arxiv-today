https://arxiv.org/abs/2504.02263

*MegaScale-Infer: Serving Mixture-of-Experts at Scale with Disaggregated Expert Parallelism* (Ruidong Zhu, Ziheng Jiang, Chao Jin, Peng Wu, Cesar A. Stuardo, Dongyang Wang, Xinlei Zhang, Huaping Zhou, Haoran Wei, Yang Cheng, Jianzhe Xiao, Xinyi Zhang, Lingjun Liu, Haibin Lin, Li-Wen Chang, Jianxi Ye, Xiao Yu, Xuanzhe Liu, Xin Jin, Xin Liu)

> Mixture-of-Experts (MoE) showcases tremendous potential to scale large language models (LLMs) with enhanced performance and reduced computational complexity. However, its sparsely activated architecture shifts feed-forward networks (FFNs) from being compute-intensive to memory-intensive during inference, leading to substantially lower GPU utilization and increased operational costs. We present MegaScale-Infer, an efficient and cost-effective system for serving large-scale MoE models. MegaScale-Infer disaggregates attention and FFN modules within each model layer, enabling independent scaling, tailored parallelism strategies, and heterogeneous deployment for both modules. To fully exploit disaggregation in the presence of MoE's sparsity, MegaScale-Infer introduces ping-pong pipeline parallelism, which partitions a request batch into micro-batches and shuttles them between attention and FFNs for inference. Combined with distinct model parallelism for each module, MegaScale-Infer effectively hides communication overhead and maximizes GPU utilization. To adapt to disaggregated attention and FFN modules and minimize data transmission overhead (e.g., token dispatch), MegaScale-Infer provides a high-performance M2N communication library that eliminates unnecessary GPU-to-CPU data copies, group initialization overhead, and GPU synchronization. Experimental results indicate that MegaScale-Infer achieves up to 1.90x higher per-GPU throughput than state-of-the-art solutions.

ByteDance의 MoE 서빙 프레임워크. Attention과 FFN을 분리하고 Pipeline Parallel로 이 둘 사이를 오가는 형태군요. 오픈소스 쪽에서는 Prefill과 Decode의 분리도 이제 도입되고 있는 상황이라는 걸 생각하면 격차가 꽤 있네요.

<english>
MoE serving framework from ByteDance. They decoupled attention and ffn and used pipeline parallel to communicate with each other. Considering open source is adopting even decoupling of prefill and decode pretty recently, there seems siginificant gap between it and company internal solution on serving frameworks.
</english>

#efficiency 