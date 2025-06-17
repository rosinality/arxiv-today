https://arxiv.org/abs/2312.17296

Structured Packing in LLM Training Improves Long Context Utilization (Konrad Staniszewski, Szymon Tworkowski, Sebastian Jaszczur, Henryk Michalewski, Łukasz Kuciński, Piotr Miłoś)

LLM 학습에 랜덤한 문서를 이어붙이는 것이 아니라 관련성 높은 문서를 이어붙이는 것으로 성능을 높이겠다는 아이디어. In-context Pretraining (https://arxiv.org/abs/2310.10638) 과 비슷하군요. 여기서는 Top-K개를 사용해서 관련성이 다양한 문서를 이어붙이는 시도를 했다는 것이 차이겠네요.

사실 가끔 관련 없는 문서도 붙이는 쪽이 모델에 필요할 수도 있겠지만, 여하간 관련성 높은 문서들을 사용해 시퀀스를 구성하는 것은 꽤 좋은 방법으로 보입니다.

#pretraining #llm #retrieval

# Links

[[231016 In-Context Pretraining.md]]