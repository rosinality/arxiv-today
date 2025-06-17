https://arxiv.org/abs/2402.04624

*MEMORYLLM: Towards Self-Updatable Large Language Models* (Yu Wang, Xiusi Chen, Jingbo Shang, Julian McAuley)

> Existing Large Language Models (LLMs) usually remain static after deployment, which might make it hard to inject new knowledge into the model. We aim to build models containing a considerable portion of self-updatable parameters, enabling the model to integrate new knowledge effectively and efficiently. To this end, we introduce MEMORYLLM, a model that comprises a transformer and a fixed-size memory pool within the latent space of the transformer. MEMORYLLM can self-update with text knowledge and memorize the knowledge injected earlier. Our evaluations demonstrate the ability of MEMORYLLM to effectively incorporate new knowledge, as evidenced by its performance on model editing benchmarks. Meanwhile, the model exhibits long-term information retention capacity, which is validated through our custom-designed evaluations and long-context benchmarks. MEMORYLLM also shows operational integrity without any sign of performance degradation even after nearly a million memory updates.

LLM에 대한 새로운 지식 추가를 학습으로 풀자는 접근. 트랜스포머 레이어 입력에 학습 가능한 임베딩들을 추가하고 이 임베딩을 학습해나가면서 오래된 임베딩을 새 임베딩으로 대체해나가는 방식입니다.

새로운 지식과 능력을 추가해나가는 문제가 반드시 풀려야 한다고 봅니다. 문제는 그 방법이네요. RAG, 혹은 KV 캐시를 보존한다거나, 혹은 모델 자체를 튜닝한다거나. 그 외에 효과적이면서도 저렴한 방법이 나올 수 있을지 궁금하네요.

#long-context #continual-learning 