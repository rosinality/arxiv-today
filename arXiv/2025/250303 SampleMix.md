https://arxiv.org/abs/2503.01506

*SampleMix: A Sample-wise Pre-training Data Mixing Strategey by Coordinating Data Quality and Diversity* (Xiangyu Xi, Deyang Kong, Jian Yang, Jiawei Yang, Zhengyu Chen, Wei Wang, Jingang Wang, Xunliang Cai, Shikun Zhang, Wei Ye)

> Existing pretraining data mixing methods for large language models (LLMs) typically follow a domain-wise methodology, a top-down process that first determines domain weights and then performs uniform data sampling across each domain. However, these approaches neglect significant inter-domain overlaps and commonalities, failing to control the global diversity of the constructed training dataset. Further, uniform sampling within domains ignores fine-grained sample-specific features, potentially leading to suboptimal data distribution. To address these shortcomings, we propose a novel sample-wise data mixture approach based on a bottom-up paradigm. This method performs global cross-domain sampling by systematically evaluating the quality and diversity of each sample, thereby dynamically determining the optimal domain distribution. Comprehensive experiments across multiple downstream tasks and perplexity assessments demonstrate that SampleMix surpasses existing domain-based methods. Meanwhile, SampleMix requires 1.4x to 2.1x training steps to achieves the baselines' performance, highlighting the substantial potential of SampleMix to optimize pre-training data.

LLM으로 측정한 문서 퀄리티에 클러스터링을 사용한 다양성을 고려한 샘플링 전략. 요즘 나오는 Deduplication 이후에 Duplication 횟수를 사용해 다시 가중치를 주는 시도와 비슷한 것 같네요.

<english>
Sampling strategy with combining document quality measured by LLMs and diversity through clustering. I think it is similar to recent trials to reweight samples using number of duplicates after deduplication.
</english>

#pretraining #corpus 