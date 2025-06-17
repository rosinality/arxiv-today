https://arxiv.org/abs/2503.15758

*ATTENTION2D: Communication Efficient Distributed Self-Attention Mechanism* (Venmugil Elango)

> Transformer-based models have emerged as a leading architecture for natural language processing, natural language generation, and image generation tasks. A fundamental element of the transformer architecture is self-attention, which allows the model to capture intricate dependencies within the data. However, the self-attention mechanism also incurs significant computational and memory costs, particularly for long sequences. In this paper, we introduce ATTENTION2D, a novel approach that exploits parallelism along two dimensions - query and key/value - of the self-attention operation. This method enables efficient distribution and parallelization of computations across multiple devices. Our approach facilitates asymptotically faster training and inference phases compared to previous methods, without relying on approximations or incurring additional computational or memory overheads. Furthermore, unlike existing techniques that struggle to scale with an increasing number of processing units, our approach effectively scales with additional processing units. Our experimental results confirm the effectiveness of our method in improving communication efficiency and scalability. Compared to Ring Attention, our approach demonstrated up to a 5x performance boost on a GPT-3-like model using 64 NVIDIA A100 GPUs across 16 nodes, and up to a 9.4x performance boost on 64 NVIDIA H100 GPUs across 64 nodes.

Query 뿐만 아니라 Key-Value 축에 대해서도 병렬적으로 연산이 가능하도록 해서 분산 처리.

<english>
Distributed processing of attention by make it parallelizable not only query, but also key-value axis.
</english>

#long-context #efficiency 