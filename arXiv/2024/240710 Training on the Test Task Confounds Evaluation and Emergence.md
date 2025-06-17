https://arxiv.org/abs/2407.07890

*Training on the Test Task Confounds Evaluation and Emergence* (Ricardo Dominguez-Olmedo, Florian E. Dorner, Moritz Hardt)

> We study a fundamental problem in the evaluation of large language models that we call training on the test task. Unlike wrongful practices like training on the test data, leakage, or data contamination, training on the test task is not a malpractice. Rather, the term describes a growing set of techniques to include task-relevant data in the pretraining stage of a language model. We demonstrate that training on the test task confounds both relative model evaluations and claims about emergent capabilities. We argue that the seeming superiority of one model family over another may be explained by a different degree of training on the test task. To this end, we propose an effective method to adjust for training on the test task by fine-tuning each model under comparison on the same task-relevant data before evaluation. We then show that instances of emergent behavior largely vanish once we adjust for training on the test task. This also applies to reported instances of emergent behavior that cannot be explained by the choice of evaluation metric. Our work promotes a new perspective on the evaluation of large language models with broad implications for benchmarking and the study of emergent capabilities.

2023년 11월을 기점으로 이전 모델과 이후 모델의 벤치마크 성능 차이가 크게 나타나는데, 이전 모델들을 벤치마크 학습셋으로 학습시키면 이 차이가 사라진다는 결과. 이는 벤치마크 데이터에 대한 오염이라기 보다는 Multiple Choice 같은 문제의 형식에 더 익숙해졌기 때문이라고 합니다. DeepSeek LLM (https://arxiv.org/abs/2401.02954) 에서 주장했던 것과 같은 맥락이겠네요.

Yi Tay가 팟캐스트에서 (https://latent.space/p/yitay) Scaling Law를 속일 수는 없다고 했던 것이 생각나네요.

#scaling-law #benchmark

# Links

[[240105 DeepSeek LLM.md]]