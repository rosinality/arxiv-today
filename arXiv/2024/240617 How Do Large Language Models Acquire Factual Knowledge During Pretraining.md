https://arxiv.org/abs/2406.11813

*How Do Large Language Models Acquire Factual Knowledge During Pretraining?* (Hoyeon Chang, Jinho Park, Seonghyeon Ye, Sohee Yang, Youngkyung Seo, Du-Seong Chang, Minjoon Seo)

> Despite the recent observation that large language models (LLMs) can store substantial factual knowledge, there is a limited understanding of the mechanisms of how they acquire factual knowledge through pretraining. This work addresses this gap by studying how LLMs acquire factual knowledge during pretraining. The findings reveal several important insights into the dynamics of factual knowledge acquisition during pretraining. First, counterintuitively, we observe that pretraining on more data shows no significant improvement in the model's capability to acquire and maintain factual knowledge. Next, there is a power-law relationship between training steps and forgetting of memorization and generalization of factual knowledge, and LLMs trained with duplicated training data exhibit faster forgetting. Third, training LLMs with larger batch sizes can enhance the models' robustness to forgetting. Overall, our observations suggest that factual knowledge acquisition in LLM pretraining occurs by progressively increasing the probability of factual knowledge presented in the pretraining data at each step. However, this increase is diluted by subsequent forgetting. Based on this interpretation, we demonstrate that we can provide plausible explanations for recently observed behaviors of LLMs, such as the poor performance of LLMs on long-tail knowledge and the benefits of deduplicating the pretraining corpus.

LLM은 어떻게 지식을 습득하는가? 특정한 지식이 포함된 텍스트에 대해 학습될 때마다 지식을 조금씩 학습하고, 이것이 누적되면서 지식이 습득된다는 분석입니다. 특정 지식을 학습한 다음 시간이 흐를수록 습득한 지식의 강도가 약해져가죠.

여러모로 생각해볼 여지를 주는 연구네요. 예를 들어 Long Tail 분포의 지식에 대해 학습시키면 꼬리에 있는 지식들은 학습 시점의 간격이 너무 멀기 때문에 제대로 학습되기 어려울 수 있습니다. 그런 의미에서 분포의 머리 부분에서 지나치게 많이 샘플링 되는 것을 막으려는 시도 (https://arxiv.org/abs/2405.15613) 가 의미가 있을 수 있겠네요.

#pretraining

# Links

[[240524 Automatic Data Curation for Self-Supervised Learning.md]]