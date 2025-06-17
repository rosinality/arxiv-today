https://arxiv.org/abs/2505.09343

*Insights into DeepSeek-V3: Scaling Challenges and Reflections on Hardware for AI Architectures* (Chenggang Zhao, Chengqi Deng, Chong Ruan, Damai Dai, Huazuo Gao, Jiashi Li, Liyue Zhang, Panpan Huang, Shangyan Zhou, Shirong Ma, Wenfeng Liang, Ying He, Yuqing Wang, Yuxuan Liu, Y.X. Wei)

> The rapid scaling of large language models (LLMs) has unveiled critical limitations in current hardware architectures, including constraints in memory capacity, computational efficiency, and interconnection bandwidth. DeepSeek-V3, trained on 2,048 NVIDIA H800 GPUs, demonstrates how hardware-aware model co-design can effectively address these challenges, enabling cost-efficient training and inference at scale. This paper presents an in-depth analysis of the DeepSeek-V3/R1 model architecture and its AI infrastructure, highlighting key innovations such as Multi-head Latent Attention (MLA) for enhanced memory efficiency, Mixture of Experts (MoE) architectures for optimized computation-communication trade-offs, FP8 mixed-precision training to unlock the full potential of hardware capabilities, and a Multi-Plane Network Topology to minimize cluster-level network overhead. Building on the hardware bottlenecks encountered during DeepSeek-V3's development, we engage in a broader discussion with academic and industry peers on potential future hardware directions, including precise low-precision computation units, scale-up and scale-out convergence, and innovations in low-latency communication fabrics. These insights underscore the critical role of hardware and model co-design in meeting the escalating demands of AI workloads, offering a practical blueprint for innovation in next-generation AI systems.

DeepSeek의 인프라 논문. DeepSeek V3에 썼던 하드웨어 벤더를 위한 제언의 확장판 느낌이군요. 연산에 대해서도 언급하긴 하지만 결국 네트워킹의 문제를 많이 언급하고 있습니다.

<english>
DeepSeek's infrastructure paper. It feels like expansion of comments for hardware vendors in DeepSeek V3. It mentions computation, but they deals a lot with networking problems.
</english>

#infrastructure #distributed-training 