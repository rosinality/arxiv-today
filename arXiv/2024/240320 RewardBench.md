https://arxiv.org/abs/2403.13787

*RewardBench: Evaluating Reward Models for Language Modeling* (Nathan Lambert, Valentina Pyatkin, Jacob Morrison, LJ Miranda, Bill Yuchen Lin, Khyathi Chandu, Nouha Dziri, Sachin Kumar, Tom Zick, Yejin Choi, Noah A. Smith, Hannaneh Hajishirzi)

> Reward models (RMs) are at the crux of successful RLHF to align pretrained models to human preferences, yet there has been relatively little study that focuses on evaluation of those reward models. Evaluating reward models presents an opportunity to understand the opaque technologies used for alignment of language models and which values are embedded in them. To date, very few descriptors of capabilities, training methods, or open-source reward models exist. In this paper, we present RewardBench, a benchmark dataset and code-base for evaluation, to enhance scientific understanding of reward models. The RewardBench dataset is a collection of prompt-win-lose trios spanning chat, reasoning, and safety, to benchmark how reward models perform on challenging, structured and out-of-distribution queries. We created specific comparison datasets for RMs that have subtle, but verifiable reasons (e.g. bugs, incorrect facts) why one answer should be preferred to another. On the RewardBench leaderboard, we evaluate reward models trained with a variety of methods, such as the direct MLE training of classifiers and the implicit reward modeling of Direct Preference Optimization (DPO), and on a spectrum of datasets. We present many findings on propensity for refusals, reasoning limitations, and instruction following shortcomings of various reward models towards a better understanding of the RLHF process.

Preference 데이터셋들을 모은 벤치마크. 그런데 사실 Preference 데이터셋들을 모아서 벤치마크를 한다는 것이 좀 미묘하죠. "무엇을 선호할 것인가"라는 것은 각각의 데이터셋이 갖는 고유한 선택이니까요.

그렇지만 예를 들어 정답 코드 vs 잘못된 코드와 같은 셋들은 보다 명확할 것 같습니다. 여담이지만 Anthropic과 OpenAI의 데이터셋이 여전히 중요한 데이터셋이라는 게 복잡한 기분을 들게 하네요.

#reward-model #benchmark 