https://arxiv.org/abs/2411.09702

*On the Surprising Effectiveness of Attention Transfer for Vision Transformers* (Alexander C. Li, Yuandong Tian, Beidi Chen, Deepak Pathak, Xinlei Chen)

> Conventional wisdom suggests that pre-training Vision Transformers (ViT) improves downstream performance by learning useful representations. Is this actually true? We investigate this question and find that the features and representations learned during pre-training are not essential. Surprisingly, using only the attention patterns from pre-training (i.e., guiding how information flows between tokens) is sufficient for models to learn high quality features from scratch and achieve comparable downstream performance. We show this by introducing a simple method called attention transfer, where only the attention patterns from a pre-trained teacher ViT are transferred to a student, either by copying or distilling the attention maps. Since attention transfer lets the student learn its own features, ensembling it with a fine-tuned teacher also further improves accuracy on ImageNet. We systematically study various aspects of our findings on the sufficiency of attention maps, including distribution shift settings where they underperform fine-tuning. We hope our exploration provides a better understanding of what pre-training accomplishes and leads to a useful alternative to the standard practice of fine-tuning

ViT의 Distillation에서 Teacher의 Attention Map을 그대로 가져오거나 Distill 하면 Teacher의 성능을 거의 재현할 수 있다는 연구. ViT에서는 좋은 Attention 패턴을 학습하는데 시간이 오래 걸린다는 결과들이 많았죠. 그런 의미에서는 자연스러운 것 같기도 합니다.

언어 모델이나 모델 크기에 차이가 있을 때는 어떨지 궁금하네요. 물론 언어 모델에서는 Attention Map을 Distill 하는 것 자체가 까다로운 일이긴 합니다만.

<english>
The study that we can recover the performance of the teacher in ViT distillation by copying attention maps of the teacher or distill it. There was many studies said that it took a long time for learning good attention patterns for ViT. So I think this could be natural in that aspect.

I wonder how this work in language models or between different model sizes. It is hard to distill attention maps in language models, however.
</english>

#distillation #vit 