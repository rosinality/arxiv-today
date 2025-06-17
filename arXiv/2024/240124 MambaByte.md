https://arxiv.org/abs/2401.13660

*MambaByte: Token-free Selective State Space Model* (Junxiong Wang, Tushaar Gangavarapu, Jing Nathan Yan, Alexander M Rush)

> Token-free language models learn directly from raw bytes and remove the bias of subword tokenization. Operating on bytes, however, results in significantly longer sequences, and standard autoregressive Transformers scale poorly in such settings. We experiment with MambaByte, a token-free adaptation of the Mamba state space model, trained autoregressively on byte sequences. Our experiments indicate the computational efficiency of MambaByte compared to other byte-level models. We also find MambaByte to be competitive with and even outperform state-of-the-art subword Transformers. Furthermore, owing to linear scaling in length, MambaByte benefits from fast inference compared to Transformers. Our findings establish the viability of MambaByte in enabling token-free language modeling.

요새 Mamba를 이미지 등에 테스트해본 결과들이 많이 나오고 있죠. 이쪽은 바이트 레벨 LM을 해본 결과이네요. 스코어가 꽤 좋습니다.

더 큰 규모에서, Associative Recall 등과 여러 벤치마크들에 대한 테스트가 필요하겠지만 스코어가 잘 나오는 사례가 있다는 것 자체가 Mamba/SSM이 갖는 뭔가 좋은 특징이 있을 수 있다는 것을 시사하는 것이 아닐까 싶습니다. 더 흥미로운 결과들이 기다려지네요.

#state-space-model #lm 