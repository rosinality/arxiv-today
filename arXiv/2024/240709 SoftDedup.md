https://arxiv.org/abs/2407.06654

*SoftDedup: an Efficient Data Reweighting Method for Speeding Up Language Model Pre-training* (Nan He, Weichen Xiong, Hanwen Liu, Yi Liao, Lei Ding, Kai Zhang, Guohua Tang, Xiao Han, Wei Yang)

> The effectiveness of large language models (LLMs) is often hindered by duplicated data in their extensive pre-training datasets. Current approaches primarily focus on detecting and removing duplicates, which risks the loss of valuable information and neglects the varying degrees of duplication. To address this, we propose a soft deduplication method that maintains dataset integrity while selectively reducing the sampling weight of data with high commonness. Central to our approach is the concept of "data commonness", a metric we introduce to quantify the degree of duplication by measuring the occurrence probabilities of samples using an n-gram model. Empirical analysis shows that this method significantly improves training efficiency, achieving comparable perplexity scores with at least a 26% reduction in required training steps. Additionally, it enhances average few-shot downstream accuracy by 1.77% when trained for an equivalent duration. Importantly, this approach consistently improves performance, even on rigorously deduplicated datasets, indicating its potential to complement existing methods and become a standard pre-training process for LLMs.

기존의 Hard Deduplication 대신 n-gram 모델로 텍스트의 확률을 추정하고 확률의 역수로 샘플링 비율을 결정하는 Soft Deduplication. 확률이 높을수록 통상적이고 자주 등장한다는 아이디어겠죠. Semantic Deduplication의 측면에서 생각할 수 있지 않을까 싶네요. (https://arxiv.org/abs/2405.15613)

#corpus #pretraining

# Links

[[240524 Automatic Data Curation for Self-Supervised Learning.md]]