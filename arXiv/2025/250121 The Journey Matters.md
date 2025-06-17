https://arxiv.org/abs/2501.12486

*The Journey Matters: Average Parameter Count over Pre-training Unifies Sparse and Dense Scaling Laws* (Tian Jin, Ahmed Imtiaz Humayun, Utku Evci, Suvinay Subramanian, Amir Yazdanbakhsh, Dan Alistarh, Gintare Karolina Dziugaite)

> Pruning eliminates unnecessary parameters in neural networks; it offers a promising solution to the growing computational demands of large language models (LLMs). While many focus on post-training pruning, sparse pre-training--which combines pruning and pre-training into a single phase--provides a simpler alternative. In this work, we present the first systematic exploration of optimal sparse pre-training configurations for LLMs through an examination of 80 unique pruning schedules across different sparsity levels and training durations. We find that initiating pruning at 25% of total training compute and concluding at 75% achieves near-optimal final evaluation loss. These findings provide valuable insights for efficient and effective sparse pre-training of LLMs. Furthermore, we propose a new scaling law that modifies the Chinchilla scaling law to use the average parameter count over pre-training. Through empirical and theoretical validation, we demonstrate that this modified scaling law accurately models evaluation loss for both sparsely and densely pre-trained LLMs, unifying scaling laws across pre-training paradigms. Our findings indicate that while sparse pre-training achieves the same final model quality as dense pre-training for equivalent compute budgets, it provides substantial benefits through reduced model size, enabling significant potential computational savings during inference.

Sparse 모델에 대한 Scaling Law. Dense 모델 학습에서 시작해 Pruning으로 점진적으로 Sparse한 모델을 만든 다음 계속 학습하는 형태의 스케줄을 사용했습니다. 학습 전체에 사용된 평균 파라미터 수를 모델 크기로 잡으면 Chinchilla Scaling Law를 적용할 수 있다고 하네요.

Sparse 모델에 대한 연구도 간간히 나오는데 하드웨어가 뒷받침 되지 않는다는 것이 늘 문제죠. TPU에서 시도를 할지 모르겠네요.

<english>
Scaling law for sparse models. They used a schedule that starts from dense model and build sparse model incrementally, and train it further. They insist that it is possible to use functional form of chinchilla scaling law if we set average number of parameters during the training as a model size.

Studies on sparse models appears occasionally but the lack of hardware backing is alway the problem. Maybe they will try to implement it in TPUs.
</english>

#sparsity #pruning #scaling-law 