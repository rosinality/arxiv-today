https://arxiv.org/abs/2502.04667

*Unveiling the Mechanisms of Explicit CoT Training: How Chain-of-Thought Enhances Reasoning Generalization* (Xinhao Yao, Ruifeng Ren, Yun Liao, Yong Liu)

> Training large language models (LLMs) with high-quality Chain-of-Thought (CoT) annotations has become a widely adopted strategy due to its significant enhancement of reasoning capabilities. To fully comprehend this approach, two questions naturally arise: (Q1) What advantages does training with CoT offer compared to training without CoT? (Q2) If there are advantages, what are the underlying mechanisms of explicit CoT training? Analyzing the advantages and mechanisms of CoT training is challenging due to the many factors involved. To address this, we conduct a detailed analysis using clear and controllable data distributions and, for the first time, reveal that CoT training offers the following advantages: (1) Training with CoT markedly improves reasoning generalization, extending it from in-distribution (ID) to both ID and out-of-distribution (OOD) scenarios, while also speeding up convergence; (2) Even when training with CoT includes a certain range of erroneous reasoning steps, it still enables the model to learn reasoning patterns, leading to systematic generalization. We further explore the underlying mechanisms from a circuit perspective: (1) The data distribution (e.g., ratio $\lambda$ and pattern) plays a crucial role in influencing the model's systematic generalization; (2) CoT training (with two-hop facts) internalizes reasoning into a two-stage generalizing circuit, where the number of stages corresponds to the explicit reasoning steps during training. Our findings elucidate the mechanisms underlying explicit CoT training and offer critical insights into tuning strategies for LLMs to achieve robust generalization.

Knowledge Triple을 사용한 CoT의 일반화 분석. 2-hop에서 CoT로 학습하면 OOD에 대한 일반화가 가능하고 3-hop 일반화는 되지 않지만 소규모 데이터로 3-hop에 대해 작동시키는 것이 가능하다는 이야기를 하고 있네요.

<english>
Analysis on CoT using knowledge triple. They found it is able to generalized to OOD when model trained on 2-hop with CoT, it is not possible to generalize to 3-hop, but it could be trained with relatively smaller number of samples.
</english>

#reasoning 