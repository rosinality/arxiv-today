https://arxiv.org/abs/2509.01649

*Distilled Pretraining: A modern lens of Data, In-Context Learning and Test-Time Scaling* (Sachin Goyal, David Lopez-Paz, Kartik Ahuja)

> In the past year, distillation has seen a renewed prominence in large language model (LLM) pretraining, exemplified by the Llama-3.2 and Gemma model families. While distillation has historically been shown to improve statistical modeling, its effects on new paradigms that are key to modern LLMs, such as test-time scaling and in-context learning, remain underexplored. In this work, we make three main contributions. First, we show that pretraining with distillation yields models that exhibit remarkably better test-time scaling. Second, we observe that this benefit comes with a trade-off: distillation impairs in-context learning capabilities, particularly the one modeled via induction heads. Third, to demystify these findings, we study distilled pretraining in a sandbox of a bigram model, which helps us isolate the common principal factor behind our observations. Finally, using these insights, we shed light on various design choices for pretraining that should help practitioners going forward.

프리트레이닝 시점의 Distillation에 대한 분석. Diversity를 향상시키나 In-context Learning에 문제가 생김 (데이터 엔트로피가 낮을 때는 노이즈를 첨가하는 것일 수 있음). 이 문제에 대해 어떻게 대응할지, RL 학습된 모델이 더 나은 Teacher일 수 있다는 결과 등등도 포함.

Analysis of distillation during pretraining. It enhances diversity but hurts in-context learning (potentially because it introduces noise when data entropy is low). This paper also shows how to address this and finds that RL-trained models could serve as better teachers.

#distillation #pretraining 