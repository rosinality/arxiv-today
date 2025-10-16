https://arxiv.org/abs/2510.13079

*GatePro: Parameter-Free Expert Selection Optimization for Mixture-of-Experts Models* (Chen Zheng, Yuhang Cai, Deyi Liu, Jin Ma, Yiyuan Ma, Yuan Yang, Jing Liu, Yutao Zeng, Xun Zhou, Siyuan Qiao)

> Modern large language models leverage Mixture-of-Experts (MoE) architectures for efficient scaling, but face a critical challenge: functionally similar experts are often selected simultaneously, creating redundant computation and limiting effective model capacity. Existing auxiliary balance loss methods improve token distribution but fail to address the underlying expert diversity problem. We introduce GatePro, a novel parameter-free method that directly promotes expert selection diversity. GatePro identifies the most similar expert pairs and introduces localized competition mechanisms, preventing redundant expert co-activation while maintaining natural expert specialization. Our comprehensive evaluation demonstrates GatePro's effectiveness across model scales and benchmarks. Analysis demonstrates GatePro's ability to achieve enhanced expert diversity, where experts develop more distinct and complementary capabilities, avoiding functional redundancy. This approach can be deployed hot-swappable during any training phase without additional learnable parameters, offering a practical solution for improving MoE effectiveness.

Gate 가중치의 유사도로 가장 유사한 Expert를 찾아낸 다음 경쟁하는 Expert에 페널티를 가해 Expert 선택의 다양성을 촉진.

Encouraging diversity in expert selection by first finding the most similar experts using similarity of gate weights then penalizing competing experts.

#moe 