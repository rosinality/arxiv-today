https://arxiv.org/abs/2407.10827

*LLM Circuit Analyses Are Consistent Across Training and Scale* (Curt Tigges, Michael Hanna, Qinan Yu, Stella Biderman)

> Most currently deployed large language models (LLMs) undergo continuous training or additional finetuning. By contrast, most research into LLMs' internal mechanisms focuses on models at one snapshot in time (the end of pre-training), raising the question of whether their results generalize to real-world settings. Existing studies of mechanisms over time focus on encoder-only or toy models, which differ significantly from most deployed models. In this study, we track how model mechanisms, operationalized as circuits, emerge and evolve across 300 billion tokens of training in decoder-only LLMs, in models ranging from 70 million to 2.8 billion parameters. We find that task abilities and the functional components that support them emerge consistently at similar token counts across scale. Moreover, although such components may be implemented by different attention heads over time, the overarching algorithm that they implement remains. Surprisingly, both these algorithms and the types of components involved therein can replicate across model scale. These results suggest that circuit analyses conducted on small models at the end of pre-training can provide insights that still apply after additional pre-training and over model scale.

트랜스포머 LM이 특정 능력을 학습하는 시점(학습량)이 모델 크기와 관계 없이 일정했다는 결과. 추가적으로 Attention Head 등의 기능이 학습에 따라 변화하지만 모델이 학습한 알고리즘은 학습 기간 동안 일정했다고.

흥미롭네요. 창발 현상과 관련지어 생각해보면 재미있지 않을까 싶습니다.

#transformer #llm #mechanistic-interpretation