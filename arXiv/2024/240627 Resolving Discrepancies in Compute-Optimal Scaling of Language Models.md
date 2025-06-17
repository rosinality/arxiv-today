https://arxiv.org/abs/2406.19146

*Resolving Discrepancies in Compute-Optimal Scaling of Language Models* (Tomer Porian, Mitchell Wortsman, Jenia Jitsev, Ludwig Schmidt, Yair Carmon)

> Kaplan et al. and Hoffmann et al. developed influential scaling laws for the optimal model size as a function of the compute budget, but these laws yield substantially different predictions. We explain the discrepancy by reproducing the Kaplan scaling law on two datasets (OpenWebText2 and RefinedWeb) and identifying three factors causing the difference: last layer computational cost, warmup duration, and scale-dependent optimizer tuning. With these factors corrected, we obtain excellent agreement with the Hoffmann et al. (i.e., "Chinchilla") scaling law. Counter to a hypothesis of Hoffmann et al., we find that careful learning rate decay is not essential for the validity of their scaling law. As a secondary result, we derive scaling laws for the optimal learning rate and batch size, finding that tuning the AdamW $\beta_2$ parameter is essential at lower batch sizes.

Kaplan Scaling Law와 Chinchilla Scaling Law를 종합하려는 시도 2. 여기서 발견한 원인은

1. Kaplan Scaling Law에서는 임베딩 파라미터를 빼버려서 LM 헤드의 FLOPS 기여분을 과소평가했다. 이쪽은 이전에 나온 논문과 통하네요. (https://arxiv.org/abs/2406.12907)
2. 작은 모델에서 Warmup이 너무 길었다.
3. 지나치게 큰 배치 크기 문제. DeepSeek LLM의 접근 (https://arxiv.org/abs/2401.02954) 을 사용해 배치 크기와 Learning Rate에 대한 Scaling Law 추정, 그리고 작은 배치 크기를 사용하는 경우 Adam β2에 대한 조정이 필요.

Chinchilla 쪽에서의 추측과는 달리 LR Decay의 영향은 크게 없었다고 하네요.

사실 지금 Compute Optimal Scaling은 그렇게 중요하지 않은 상황인 듯 합니다만 Scaling Law 추정 과정에서 주의해야 할 부분들을 밝혀준다는 점에서는 중요한 가이드일 듯 하네요.

#scaling-law

# Links

[[240105 DeepSeek LLM.md]]
[[240612 Reconciling Kaplan and Chinchilla Scaling Laws.md]]