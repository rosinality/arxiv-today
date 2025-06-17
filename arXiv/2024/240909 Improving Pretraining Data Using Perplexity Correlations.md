https://arxiv.org/abs/2409.05816

*Improving Pretraining Data Using Perplexity Correlations* (Tristan Thrush, Christopher Potts, Tatsunori Hashimoto)

> Quality pretraining data is often seen as the key to high-performance language models. However, progress in understanding pretraining data has been slow due to the costly pretraining runs required for data selection experiments. We present a framework that avoids these costs and selects high-quality pretraining data without any LLM training of our own. Our work is based on a simple observation: LLM losses on many pretraining texts are correlated with downstream benchmark performance, and selecting high-correlation documents is an effective pretraining data selection method. We build a new statistical framework for data selection centered around estimates of perplexity-benchmark correlations and perform data selection using a sample of 90 LLMs taken from the Open LLM Leaderboard on texts from tens of thousands of web domains. In controlled pretraining experiments at the 160M parameter scale on 8 benchmarks, our approach outperforms DSIR on every benchmark, while matching the best data selector found in DataComp-LM, a hand-engineered bigram classifier.

도메인에 대한 Likelihood와 벤치마크의 성능 사이의  상관계수를 통해 벤치마크에 가장 도움이 되는 도메인을 Positive로 하는 분류기를 학습시키고 이를 통해 샘플링한다는 아이디어. 도메인과 벤치마크의 관계를 예측한 연구의 연장선상이라고 할 수있겠네요. (https://arxiv.org/abs/2404.09937)

저는 좋은 LLM을 만들기 위해서는 벤치마크에 무심해야 한다고 생각합니다. 그렇지만 도메인 비율 설정이나 모델 기반 퀄리티 필터링에 대해 좀 더 나은 접근이 필요한 것도 사실이겠죠.

#corpus

# Links

[[240415 Compression Represents Intelligence Linearly.md]]