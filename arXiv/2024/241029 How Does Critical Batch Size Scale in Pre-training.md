https://arxiv.org/abs/2410.21676

*How Does Critical Batch Size Scale in Pre-training?* (Hanlin Zhang, Depen Morwani, Nikhil Vyas, Jingfeng Wu, Difan Zou, Udaya Ghai, Dean Foster, Sham Kakade)

> Training large-scale models under given resources requires careful design of parallelism strategies. In particular, the efficiency notion of critical batch size, concerning the compromise between time and compute, marks the threshold beyond which greater data parallelism leads to diminishing returns. To operationalize it, we propose a measure of CBS and pre-train a series of auto-regressive language models, ranging from 85 million to 1.2 billion parameters, on the C4 dataset. Through extensive hyper-parameter sweeps and careful control on factors such as batch size, momentum, and learning rate along with its scheduling, we systematically investigate the impact of scale on CBS. Then we fit scaling laws with respect to model and data sizes to decouple their effects. Overall, our results demonstrate that CBS scales primarily with data size rather than model size, a finding we justify theoretically through the analysis of infinite-width limits of neural networks and infinite-dimensional least squares regression. Of independent interest, we highlight the importance of common hyper-parameter choices and strategies for studying large-scale pre-training beyond fixed training durations.

Crticial Batch Size에 대한 Scaling Law. 결론은 모델 크기에 비해 데이터 크기 증가에 따라 Critical Batch Size가 증가한다는 것이군요. 배치 크기 - 토큰 길이에 따른 관계라거나 LR 스케줄을 대체하는 Constant + EWA 등등 재미있는 부분들이 많습니다.

<english>
Scaling law for critical batch sizes. The conclusion is critical batch sizes are increasing with data sizes rather than model sizes. There are many interesting explorations like relationships between batch sizes and token lengths, and constant learning rate + EWA which replaces learning rate scheduling.
</english>

#scaling-law #hyperparameter 