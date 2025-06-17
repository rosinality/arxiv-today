https://arxiv.org/abs/2310.10638

In-Context Pretraining: Language Modeling Beyond Document Boundaries (Weijia Shi, Sewon Min, Maria Lomeli, Chunting Zhou, Margaret Li, Victoria Lin, Noah A. Smith, Luke Zettlemoyer, Scott Yih, Mike Lewis)

LM 프리트레이닝 시에 문서를 랜덤하게 연결하는 대신 retrieval로 관계가 있는 문서끼리 연결해서 학습시키면 어떨까 하는 아이디어군요. 문서 경계를 넘어서는 관계를 학습할 수 있다는 것 자체도 플러스이고, 학습 과정에서 큰 정보가 없는 문서에 대해 attention을 계산하는 것이 무의미하다고 보면 그 자체로도 학습 효율성에 도움이 될 수 있겠군요.

이 방법으로 특별히 문제가 될 만한 부분이 없어 보인다는 점에서 꽤 유용한 개선이 되지 않을까 싶습니다. 배치 간에 correlation을 만드는 것은 RNN LM 시절의 트릭인데 (여기서는 배치 내이긴 하지만) 비슷한 아이디어를 보게 된 것 같아 반갑네요.

#pretraining #lm #retrieval 