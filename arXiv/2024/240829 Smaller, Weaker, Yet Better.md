https://arxiv.org/abs/2408.16737

*Smaller, Weaker, Yet Better: Training LLM Reasoners via Compute-Optimal Sampling* (Hritik Bansal, Arian Hosseini, Rishabh Agarwal, Vinh Q. Tran, Mehran Kazemi)

> Training on high-quality synthetic data from strong language models (LMs) is a common strategy to improve the reasoning performance of LMs. In this work, we revisit whether this strategy is compute-optimal under a fixed inference budget (e.g., FLOPs). To do so, we investigate the trade-offs between generating synthetic data using a stronger but more expensive (SE) model versus a weaker but cheaper (WC) model. We evaluate the generated data across three key metrics: coverage, diversity, and false positive rate, and show that the data from WC models may have higher coverage and diversity, but also exhibit higher false positive rates. We then finetune LMs on data from SE and WC models in different settings: knowledge distillation, self-improvement, and a novel weak-to-strong improvement setup where a weaker LM teaches reasoning to a stronger LM. Our findings reveal that models finetuned on WC-generated data consistently outperform those trained on SE-generated data across multiple benchmarks and multiple choices of WC and SE models. These results challenge the prevailing practice of relying on SE models for synthetic data generation, suggesting that WC may be the compute-optimal approach for training advanced LM reasoners.

작은 모델로 더 많이 생성한 데이터가 큰 모델로 조금 생성한 데이터보다 큰 모델에 대한 튜닝에 대해서도 더 유리할 수 있다는 주장. 물론 이는 최종 답을 사용해서 데이터를 필터링 할 수 있었던 덕이 있었겠죠.

큰 모델의 다양성 문제 때문에 큰 모델로 생성한 데이터가 문제가 되는 경우도 있는데 (https://arxiv.org/abs/2310.13798) 이쪽은 포스트트레이닝을 거친 모델이니 좀 다르긴 합니다.

#synthetic-data

# Links

[[231020 Specific versus General Principles for Constitutional AI.md]]