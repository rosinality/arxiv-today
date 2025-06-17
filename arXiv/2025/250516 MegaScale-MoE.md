https://arxiv.org/abs/2505.11432

*MegaScale-MoE: Large-Scale Communication-Efficient Training of Mixture-of-Experts Models in Production* (Chao Jin, Ziheng Jiang, Zhihao Bai, Zheng Zhong, Juncai Liu, Xiang Li, Ningxin Zheng, Xi Wang, Cong Xie, Wen Heng, Yiyuan Ma, Wenlei Bao, Size Zheng, Yanghua Peng, Haibin Lin, Xuanzhe Liu, Xin Jin, Xin Liu)

> We present MegaScale-MoE, a production system tailored for the efficient training of large-scale mixture-of-experts (MoE) models. MoE emerges as a promising architecture to scale large language models (LLMs) to unprecedented sizes, thereby enhancing model performance. However, existing MoE training systems experience a degradation in training efficiency, exacerbated by the escalating scale of MoE models and the continuous evolution of hardware. Recognizing the pivotal role of efficient communication in enhancing MoE training, MegaScale-MoE customizes communication-efficient parallelism strategies for attention and FFNs in each MoE layer and adopts a holistic approach to overlap communication with computation at both inter- and intra-operator levels. Additionally, MegaScale-MoE applies communication compression with adjusted communication patterns to lower precision, further improving training efficiency. When training a 352B MoE model on 1,440 NVIDIA Hopper GPUs, MegaScale-MoE achieves a training throughput of 1.41M tokens/s, improving the efficiency by 1.88$\times$ compared to Megatron-LM. We share our operational experience in accelerating MoE training and hope that by offering our insights in system design, this work will motivate future research in MoE systems.

바이트댄스의 MoE 학습 프레임워크군요. MoE 레이어의 Forward/Backward 과정을 분해하고 손질해서 Computation/Communication Overlap을 유도하고, GroupedGEMM과 통신을 타일 단위로 Overlap했군요.

<english>
ByteDance's MoE training framework. They reorganized forward and backward steps of MoE layers to induce computation-communication overlap, and did intra operator overlap for GroupedGEMM and communication based on tile level overlapping.
</english>

#moe #efficiency 