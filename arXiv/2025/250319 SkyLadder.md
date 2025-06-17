https://arxiv.org/abs/2503.15450

*SkyLadder: Better and Faster Pretraining via Context Window Scheduling* (Tongyao Zhu, Qian Liu, Haonan Wang, Shiqi Chen, Xiangming Gu, Tianyu Pang, Min-Yen Kan)

> Recent advancements in LLM pretraining have featured ever-expanding context windows to process longer sequences. However, our pilot study reveals that models pretrained with shorter context windows consistently outperform their long-context counterparts under a fixed token budget. This finding motivates us to explore an optimal context window scheduling strategy to better balance long-context capability with pretraining efficiency. To this end, we propose SkyLadder, a simple yet effective approach that implements a short-to-long context window transition. SkyLadder preserves strong standard benchmark performance, while matching or exceeding baseline results on long context tasks. Through extensive experiments, we pre-train 1B-parameter models (up to 32K context) and 3B-parameter models (8K context) on 100B tokens, demonstrating that SkyLadder yields consistent gains of up to 3.7% on common benchmarks, while achieving up to 22% faster training speeds compared to baselines. The code is at https://github.com/sail-sg/SkyLadder.

Context Window가 작을 때 학습이 더 빠르다는 것을 기반으로 한 프리트레이닝에서 Context Window를 점진적으로 늘려나가는 아이디어. 완전히 Shortformer 시대의 아이디어네요. (https://arxiv.org/abs/2012.15832) 학습 과정에서 배치 크기를 늘려나가는 것은 요즘 흔한 트릭이니 그쪽으로 생각해도 될 것 같습니다.

<english>
Based on observation of training is faster when context window is smaller, the authors suggest the idea of gradually increasing context window during pretraining. It is the idea of the era of shortformer (https://arxiv.org/abs/2012.15832). As it is common trick to gradually increase batch sizes during training process nowadays we can think this in that way.
</english>

#pretraining #long-context 