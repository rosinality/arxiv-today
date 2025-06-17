https://drive.google.com/file/d/17iGn3c-sYNiLyRSY-A85QOzgzGnGiVI3/view

StarCoder 2와 The Stack v2가 나왔습니다. 이전과는 달리 Permissive 라이선스 뿐만 아니라 라이선스가 없는 사례도 포함시켜서 전체 데이터 용량이 7배 정도로 증가했습니다. 거기에 Pull Request와 문서들, LLVM IR, 코드와 수학 데이터셋, 자연어 데이터셋들까지 포함시켰습니다.

이걸 모아서 600 - 900B 가량의 데이터셋을 구성한 다음 3 - 4T 정도 학습시켰네요. 여기까지는 좋은데...벤치마크 스코어 여기저기에서 2T 학습 모델 DeepSeek-Coder에 밀리는 모습을 보여줍니다. 물론 Reasoning이나 Low Resource Language에 대한 성능 등 우세한 부분도 있긴 하지만요. 저자들에게도 좀 당황스러운 결과인 듯 하네요.

얼핏 봐서는 Markdown 같은 문서가 많이 들어갔다는 것, 퀄리티 필터링에서의 차이, 그리고 Dependency에 대한 고려 등의 차이가 눈에 띄긴 합니다. 원인이 무엇일지 찾아보는 것이 필요할 듯 하네요.

#llm #code 