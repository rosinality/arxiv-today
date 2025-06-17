https://arxiv.org/abs/2502.17356

*Distributional Scaling Laws for Emergent Capabilities* (Rosie Zhao, Tian Qin, David Alvarez-Melis, Sham Kakade, Naomi Saphra)

> In this paper, we explore the nature of sudden breakthroughs in language model performance at scale, which stands in contrast to smooth improvements governed by scaling laws. While advocates of "emergence" view abrupt performance gains as capabilities unlocking at specific scales, others have suggested that they are produced by thresholding effects and alleviated by continuous metrics. We propose that breakthroughs are instead driven by continuous changes in the probability distribution of training outcomes, particularly when performance is bimodally distributed across random seeds. In synthetic length generalization tasks, we show that different random seeds can produce either highly linear or emergent scaling trends. We reveal that sharp breakthroughs in metrics are produced by underlying continuous changes in their distribution across seeds. Furthermore, we provide a case study of inverse scaling and show that even as the probability of a successful run declines, the average performance of a successful run continues to increase monotonically. We validate our distributional scaling framework on realistic settings by measuring MMLU performance in LLM populations. These insights emphasize the role of random variation in the effect of scale on LLM capabilities.

모델의 능력이 Emergent하게 발생하는 것이 사실 랜덤 시드에 따른 모델의 성능 분포가 Bimodal하기 때문에 발생할 수 있다는 분석. 모델의 분포가 문제가 된다는 것이죠. 흥미롭네요.

<english>
The author says emergent phenomena of model capabilities might arise from the bimodal distribution of model abilities on random seeds. That means distribution of models became a problem. Interesting.
</english>

#scaling-law #llm 