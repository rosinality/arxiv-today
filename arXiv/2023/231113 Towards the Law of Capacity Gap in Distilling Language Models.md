https://arxiv.org/abs/2311.07052

Towards the Law of Capacity Gap in Distilling Language Models (Chen Zhang, Dawei Song, Zheyu Ye, Yan Gao)

LM에서 distillation은 잘 안 되는 것으로 알려져 있죠. 여기서는 한 가지 이슈인 capacity gap 문제를 논하고 있네요. 더 큰 모델을 teacher로 쓰는 것이 반드시 좋지 않다는 것입니다. 여기서는 그걸 그냥 받아들이고 그래서 어느 정도 큰 규모의 teacher를 쓰는 것이 좋은가? 하는 질문을 합니다. structured pruning으로 임의의 작은 모델을 만들어서 테스트하는 식인데 50% ~ 60% sparsity 정도가 최선이라고 봤네요.

#distillation 