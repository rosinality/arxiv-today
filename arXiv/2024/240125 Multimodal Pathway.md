https://arxiv.org/abs/2401.14405

*Multimodal Pathway: Improve Transformers with Irrelevant Data from Other Modalities* (Yiyuan Zhang, Xiaohan Ding, Kaixiong Gong, Yixiao Ge, Ying Shan, Xiangyu Yue)

> We propose to improve transformers of a specific modality with irrelevant data from other modalities, e.g., improve an ImageNet model with audio or point cloud datasets. We would like to highlight that the data samples of the target modality are irrelevant to the other modalities, which distinguishes our method from other works utilizing paired (e.g., CLIP) or interleaved data of different modalities. We propose a methodology named Multimodal Pathway - given a target modality and a transformer designed for it, we use an auxiliary transformer trained with data of another modality and construct pathways to connect components of the two models so that data of the target modality can be processed by both models. In this way, we utilize the universal sequence-to-sequence modeling abilities of transformers obtained from two modalities. As a concrete implementation, we use a modality-specific tokenizer and task-specific head as usual but utilize the transformer blocks of the auxiliary model via a proposed method named Cross-Modal Re-parameterization, which exploits the auxiliary weights without any inference costs. On the image, point cloud, video, and audio recognition tasks, we observe significant and consistent performance improvements with irrelevant data from other modalities. The code and models are available at https://github.com/AILab-CVC/M2PT.

완전히 동떨어진 모달리티를 결합했을 때에도 상승 효과가 있을지에 대한 탐색. 텍스트에 대해 학습한 모델이 이미지 학습에도 도움이 된다고 하는 결과들과 연관지을 수 있겠네요.

서로 다른 모달리티에 대한 모델을 결합하는 방식이 특이한데...일단 각 모달리티에 대해 Self Supervision으로 학습한 모델들의 Weight를 선형 결합한 다음 과제에 대해 파인튜닝 하는 방법을 썼습니다.

최근 나온 모델 결합 시도들이 생각나네요. (https://arxiv.org/abs/2401.02412, https://arxiv.org/abs/2401.08525) 동일한 모델 하나에 모든 모달리티를 집어넣는 것이 이상적이지 않나 생각하지만 동시에 모델 결합이라는 시도도 생각해 볼 만하다 싶습니다.

#multimodal

# Links

[[240104 LLM Augmented LLMs.md]]
[[240116 GATS.md]]