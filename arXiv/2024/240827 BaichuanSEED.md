https://arxiv.org/abs/2408.15079

*BaichuanSEED: Sharing the Potential of ExtensivE Data Collection and Deduplication by Introducing a Competitive Large Language Model Baseline* (Guosheng Dong, Da Pan, Yiding Sun, Shusen Zhang, Zheng Liang, Xin Wu, Yanjun Shen, Fan Yang, Haoze Sun, Tianpeng Li, Mingan Lin, Jianhua Xu, Yufan Zhang, Xiaonan Nie, Lei Su, Bingning Wang, Wentao Zhang, Jiaxin Mao, Zenan Zhou, Weipeng Chen)

> The general capabilities of Large Language Models (LLM) highly rely on the composition and selection on extensive pretraining datasets, treated as commercial secrets by several institutions. To mitigate this issue, we open-source the details of a universally applicable data processing pipeline and validate its effectiveness and potential by introducing a competitive LLM baseline. Specifically, the data processing pipeline consists of broad collection to scale up and reweighting to improve quality. We then pretrain a 7B model BaichuanSEED with 3T tokens processed by our pipeline without any deliberate downstream task-related optimization, followed by an easy but effective supervised fine-tuning stage. BaichuanSEED demonstrates consistency and predictability throughout training and achieves comparable performance on comprehensive benchmarks with several commercial advanced large language models, such as Qwen1.5 and Llama3. We also conduct several heuristic experiments to discuss the potential for further optimization of downstream tasks, such as mathematics and coding.

Baichuan 쪽에서 자신들의 프리트레이닝 데이터셋 구축 파이프라인에 대한 디테일을 공개했군요. 재미있는 점들은,

1. Global Deduplication. FineWeb에서는 Global Deduplication이 별로였다고 하지만 Global Deduplication을 하는 사례는 계속 나오네요. Llama 3도 Global Deduplication을 했었죠.
2. 사람이 직접 어노테이션한 퀄리티 필터. 이것도 가끔 등장하는군요. (https://arxiv.org/abs/2403.17297) 사람이 판단하기에 좋은 데이터가 정말로 좋은 데이터인지는 다른 문제이긴 하지만요. (https://arxiv.org/abs/2406.11794)
3. 서적이나 논문 데이터를 적지 않은 분량 수집 및 사용. 대략 750B 정도를 학습에 썼네요.

#corpus #pretraining

# Links

[[240619 DataComp-LM.md]]
[[240326 InternLM2 Technical Report.md]]