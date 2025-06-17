https://arxiv.org/abs/2401.13160

*SpacTor-T5: Pre-training T5 Models with Span Corruption and Replaced Token Detection* (Ke Ye, Heinrich Jiang, Afshin Rostamizadeh, Ayan Chakrabarti, Giulia DeSalvo, Jean-François Kagy, Lazaros Karydas, Gui Citovsky, Sanjiv Kumar)

> Pre-training large language models is known to be extremely resource intensive and often times inefficient, under-utilizing the information encapsulated in the training text sequences. In this paper, we present SpacTor, a new training procedure consisting of (1) a hybrid objective combining span corruption (SC) and token replacement detection (RTD), and (2) a two-stage curriculum that optimizes the hybrid objective over the initial $\tau$ iterations, then transitions to standard SC loss. We show empirically that the effectiveness of the hybrid objective is tied to the two-stage pre-training schedule, and provide extensive analysis on why this is the case. In our experiments with encoder-decoder architectures (T5) on a variety of NLP tasks, SpacTor-T5 yields the same downstream performance as standard SC pre-training, while enabling a 50% reduction in pre-training iterations and 40% reduction in total FLOPs. Alternatively, given the same amount of computing budget, we find that SpacTor results in significantly improved downstream benchmark performance.

구글은 T5를 참 좋아한다 싶네요. Span Corruption에 ELECTRA스럽게 마스킹된 토큰 예측을 붙여서 인코더는 Generator가 생성한 토큰을 검출하고 디코더는 Span을 예측하게 했네요. 까다롭게도 학습 중에서 이 Objective를 계속 사용할 수는 없고 초기에만 사용한 다음 Span Corrpution으로 나머지 학습을 진행해야 합니다.

#mlm 