https://arxiv.org/abs/2406.06144

*Language Models Resist Alignment* (Jiaming Ji, Kaile Wang, Tianyi Qiu, Boyuan Chen, Jiayi Zhou, Changye Li, Hantao Lou, Yaodong Yang)

> Large language models (LLMs) may exhibit undesirable behaviors. Recent efforts have focused on aligning these models to prevent harmful generation. Despite these efforts, studies have shown that even a well-conducted alignment process can be easily circumvented, whether intentionally or accidentally. Do alignment fine-tuning have robust effects on models, or are merely superficial? In this work, we answer this question through both theoretical and empirical means. Empirically, we demonstrate the elasticity of post-alignment models, i.e., the tendency to revert to the behavior distribution formed during the pre-training phase upon further fine-tuning. Using compression theory, we formally derive that such fine-tuning process \textit{disproportionately} undermines alignment compared to pre-training, potentially by orders of magnitude. We conduct experimental validations to confirm the presence of elasticity across models of varying types and sizes. Specifically, we find that model performance declines rapidly before reverting to the pre-training distribution, after which the rate of decline drops significantly. We further reveal that elasticity positively correlates with increased model size and the expansion of pre-training data. Our discovery signifies the importance of taming the inherent elasticity of LLMs, thereby overcoming the resistance of LLMs to alignment finetuning.

정렬 과정을 거친 모델의 정렬을 깨는 것이 왜 그렇게 쉬운가? 에 대한 탐구. 프리트레이닝 데이터셋의 크기가 훨씬 크기 때문에 포스트트레이닝을 거친 모델을 프리트레이닝 분포로 돌리는 것이 비교적 쉽다는 이야기를 하고 있습니다.

반대로 생각하면 포스트트레이닝 과정에서 프리트레이닝에서 학습된 것들이 보존되기 때문에 포스트트레이닝이 의미가 있는 것이라고 할 수도 있겠죠. (그리고 이런 관점에서 포스트트레이닝에 접근하는 것이 더 유용하다는 생각도 합니다.)

#alignment #posttraining