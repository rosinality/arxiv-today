https://arxiv.org/abs/2404.18824

*Benchmarking Benchmark Leakage in Large Language Models* (Ruijie Xu, Zengzhi Wang, Run-Ze Fan, Pengfei Liu)

> Amid the expanding use of pre-training data, the phenomenon of benchmark dataset leakage has become increasingly prominent, exacerbated by opaque training processes and the often undisclosed inclusion of supervised data in contemporary Large Language Models (LLMs). This issue skews benchmark effectiveness and fosters potentially unfair comparisons, impeding the field's healthy development. To address this, we introduce a detection pipeline utilizing Perplexity and N-gram accuracy, two simple and scalable metrics that gauge a model's prediction precision on benchmark, to identify potential data leakages. By analyzing 31 LLMs under the context of mathematical reasoning, we reveal substantial instances of training even test set misuse, resulting in potentially unfair comparisons. These findings prompt us to offer several recommendations regarding model documentation, benchmark setup, and future evaluations. Notably, we propose the "Benchmark Transparency Card" to encourage clear documentation of benchmark utilization, promoting transparency and healthy developments of LLMs. we have made our leaderboard, pipeline implementation, and model predictions publicly available, fostering future research.

벤치마크 데이터셋에 대한 오염 검증. Perplexity와 n-gram을 평가 척도로 해서 데이터셋과 데이터셋을 Paraphrasing한 데이터셋 사이의 스코어 차이를 사용해서 평가했습니다. 논문에서 제안하는 것은 벤치마크 학습 데이터셋 같은 걸 썼다는 것 자체는 문제는 아닐 수 있는데 썼으면 썼다고 하는 것이 좋지 않겠는가군요.

#benchmark 