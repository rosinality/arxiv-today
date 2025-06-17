https://arxiv.org/abs/2402.09668

*How to Train Data-Efficient LLMs* (Noveen Sachdeva, Benjamin Coleman, Wang-Cheng Kang, Jianmo Ni, Lichan Hong, Ed H. Chi, James Caverlee, Julian McAuley, Derek Zhiyuan Cheng)

> The training of large language models (LLMs) is expensive. In this paper, we study data-efficient approaches for pre-training LLMs, i.e., techniques that aim to optimize the Pareto frontier of model quality and training resource/data consumption. We seek to understand the tradeoffs associated with data selection routines based on (i) expensive-to-compute data-quality estimates, and (ii) maximization of coverage and diversity-based measures in the feature space. Our first technique, Ask-LLM, leverages the zero-shot reasoning capabilities of instruction-tuned LLMs to directly assess the quality of a training example. To target coverage, we propose Density sampling, which models the data distribution to select a diverse sample. In our comparison of 19 samplers, involving hundreds of evaluation tasks and pre-training runs, we find that Ask-LLM and Density are the best methods in their respective categories. Coverage sampling can recover the performance of the full data, while models trained on Ask-LLM data consistently outperform full-data training -- even when we reject 90% of the original dataset, while converging up to 70% faster.

LLM 프리트레이닝 데이터셋을 필터링하기 위한 방법 제안. 한 가지는 임베딩을 사용해 분포 밀도로 분포에 대한 커버는 유지하면서 중복을 제거하는 평이한(?) 방법인 Density이고, 다른 방법은 LLM에게 프리트레이닝 데이터로 쓸만하겠냐고 물어보는 Ask-LLM 입니다.

실험이 굉장히 많은데 결론은 Ask-LLM이 (비싸다는 것을 제외하면) 전체 데이터 사용 이상으로 성능을 향상시키는 것에 유망한 방법이라고 보고 있네요.

#dataset 