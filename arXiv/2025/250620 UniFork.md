https://arxiv.org/abs/2506.17202

*UniFork: Exploring Modality Alignment for Unified Multimodal Understanding and Generation* (Teng Li, Quanfeng Lu, Lirui Zhao, Hao Li, Xizhou Zhu, Yu Qiao, Jun Zhang, Wenqi Shao)

> Unified image understanding and generation has emerged as a promising paradigm in multimodal artificial intelligence. Despite recent progress, the optimal architectural design for such unified models remains an open challenge. In this work, we start by analyzing the modality alignment behaviors of task-specific expert models for understanding and generation, as well as current unified models. Our analysis reveals a crucial observation: understanding tasks benefit from a progressively increasing modality alignment across network depth, which helps build up semantic information for better comprehension; In contrast, generation tasks follow a different trend: modality alignment increases in the early layers but decreases in the deep layers to recover spatial details. These divergent alignment patterns create a fundamental conflict in fully shared Transformer backbones, where a uniform representational flow often leads to performance compromises across two tasks. Motivated by this finding, we introduce UniFork, a novel Y-shaped architecture that shares the shallow layers for cross-task representation learning, while employing task-specific branches in deeper layers to avoid task interference. This design effectively balances shared learning and task specialization. Through extensive ablation experiments, we demonstrate that Unifork consistently outperforms conventional fully shared Transformer architectures, and achieves performance on par with or better than task-specific models.

이미지 생성과 인식이 서로 충돌하는 과제라는 분석이군요.

<english>
The analysis that image understanding and generation is conflicting task.
</english>

#multimodal #image-generation 