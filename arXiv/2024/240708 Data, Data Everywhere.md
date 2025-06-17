https://arxiv.org/abs/2407.06380

*Data, Data Everywhere: A Guide for Pretraining Dataset Construction* (Jupinder Parmar, Shrimai Prabhumoye, Joseph Jennings, Bo Liu, Aastha Jhunjhunwala, Zhilin Wang, Mostofa Patwary, Mohammad Shoeybi, Bryan Catanzaro)

> The impressive capabilities of recent language models can be largely attributed to the multi-trillion token pretraining datasets that they are trained on. However, model developers fail to disclose their construction methodology which has lead to a lack of open information on how to develop effective pretraining sets. To address this issue, we perform the first systematic study across the entire pipeline of pretraining set construction. First, we run ablations on existing techniques for pretraining set development to identify which methods translate to the largest gains in model accuracy on downstream evaluations. Then, we categorize the most widely used data source, web crawl snapshots, across the attributes of toxicity, quality, type of speech, and domain. Finally, we show how such attribute information can be used to further refine and improve the quality of a pretraining set. These findings constitute an actionable set of steps that practitioners can use to develop high quality pretraining sets.

프리트레이닝 코퍼스에 대한 큐레이션 실험. 여기서는 DSIR (https://arxiv.org/abs/2302.03169) 같은 샘플링, UniMax (https://arxiv.org/abs/2304.09151) 같은 샘플링 비율 설정, 그리고 도메인을 구분한 다음 도메인별 샘플링 등을 시도했습니다. 재미있네요.

#corpus #pretraining

# Links

[[230418 UniMax.md]]