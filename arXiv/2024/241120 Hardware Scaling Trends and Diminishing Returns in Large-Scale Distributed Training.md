https://arxiv.org/abs/2411.13055

*Hardware Scaling Trends and Diminishing Returns in Large-Scale Distributed Training* (Jared Fernandez, Luca Wehrstedt, Leonid Shamis, Mostafa Elhoushi, Kalyan Saladi, Yonatan Bisk, Emma Strubell, Jacob Kahn)

> Dramatic increases in the capabilities of neural network models in recent years are driven by scaling model size, training data, and corresponding computational resources. To develop the exceedingly large networks required in modern applications, such as large language models (LLMs), model training is distributed across tens of thousands of hardware accelerators (e.g. GPUs), requiring orchestration of computation and communication across large computing clusters. In this work, we demonstrate that careful consideration of hardware configuration and parallelization strategy is critical for effective (i.e. compute- and cost-efficient) scaling of model size, training data, and total computation. We conduct an extensive empirical study of the performance of large-scale LLM training workloads across model size, hardware configurations, and distributed parallelization strategies. We demonstrate that: (1) beyond certain scales, overhead incurred from certain distributed communication strategies leads parallelization strategies previously thought to be sub-optimal in fact become preferable; and (2) scaling the total number of accelerators for large model training quickly yields diminishing returns even when hardware and parallelization strategies are properly optimized, implying poor marginal performance per additional unit of power or GPU-hour.

클러스터 크기가 증가할수록 연산과 중첩할 수 없는 통신 비용이 학습 스루풋을 지배한다는 분석. 하드웨어가 발전할수록 연산력 증가에 비해 통신 속도의 증가는 더디기 때문에 상황이 더 안 좋아진다는 이야기입니다. 블랙웰에서 NVLink로 72개 GPU가 연결된 것이 도움이 될지도 모르겠네요.

<english>
As scale of cluter increases, then communication costs that cannot be overlapped with computation dominates overall training throughputs. As increase of communication bandwidth is slower compared to computational power, so overall situation will became worse. Maybe NVLink with connecting 72 GPUs, introduced in Blackwell can be helpful for this.
</english>

#scaling #parallelism #efficient-training 