https://arxiv.org/abs/2405.09673

*LoRA Learns Less and Forgets Less* (Dan Biderman, Jose Gonzalez Ortiz, Jacob Portes, Mansheej Paul, Philip Greengard, Connor Jennings, Daniel King, Sam Havens, Vitaliy Chiley, Jonathan Frankle, Cody Blakeney, John P. Cunningham)

> Low-Rank Adaptation (LoRA) is a widely-used parameter-efficient finetuning method for large language models. LoRA saves memory by training only low rank perturbations to selected weight matrices. In this work, we compare the performance of LoRA and full finetuning on two target domains, programming and mathematics. We consider both the instruction finetuning (≈100K prompt-response pairs) and continued pretraining (≈10B unstructured tokens) data regimes. Our results show that, in most settings, LoRA substantially underperforms full finetuning. Nevertheless, LoRA exhibits a desirable form of regularization: it better maintains the base model's performance on tasks outside the target domain. We show that LoRA provides stronger regularization compared to common techniques such as weight decay and dropout; it also helps maintain more diverse generations. We show that full finetuning learns perturbations with a rank that is 10-100X greater than typical LoRA configurations, possibly explaining some of the reported gaps. We conclude by proposing best practices for finetuning with LoRA.

LoRA가 학습량이 적은 만큼 모델의 기존 성능 저하도 약하다는 연구. 사실 학습 성능과 성능 저하의 트레이드오프, 즉 파레토 커브에서 어느 위치에 있는가가 중요하겠죠. 조금 허무하지만 파레토 커브에서는 대체로 풀 파인튜닝과 비슷하고 가끔 LoRA가 더 나은 위치에 있는 경우가 존재하네요.

#finetuning 