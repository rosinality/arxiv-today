https://arxiv.org/abs/2402.01566

*Boximator: Generating Rich and Controllable Motions for Video Synthesis* (Jiawei Wang, Yuchen Zhang, Jiaxin Zou, Yan Zeng, Guoqiang Wei, Liping Yuan, Hang Li)

> Generating rich and controllable motion is a pivotal challenge in video synthesis. We propose Boximator, a new approach for fine-grained motion control. Boximator introduces two constraint types: hard box and soft box. Users select objects in the conditional frame using hard boxes and then use either type of boxes to roughly or rigorously define the object's position, shape, or motion path in future frames. Boximator functions as a plug-in for existing video diffusion models. Its training process preserves the base model's knowledge by freezing the original weights and training only the control module. To address training challenges, we introduce a novel self-tracking technique that greatly simplifies the learning of box-object correlations. Empirically, Boximator achieves state-of-the-art video quality (FVD) scores, improving on two base models, and further enhanced after incorporating box constraints. Its robust motion controllability is validated by drastic increases in the bounding box alignment metric. Human evaluation also shows that users favor Boximator generation results over the base model.

https://boximator.github.io/

이미지 생성도 그렇지만 영상 생성에는 생성 결과를 어떻게 통제할 것인가가 중요한 요소가 될 것 같은데요, 그 방향에서 재미있는 연구네요. 박스로 객체를 지정하고 박스의 움직임을 설정해서 객체의 움직임을 지정할 수 있게 했네요. DragGAN (https://arxiv.org/abs/2305.10973) 같은 아이디어가 떠오릅니다.

Video Diffusion에 박스 조건 입력을 추가하고 트래커로 만든 데이터셋에 대해 이미지와 박스를 같이 생성하게 해서 트래킹 능력을 향상시킨 다음 추론 시점에서 박스 입력을 주는 방식입니다.

#video-generation #controllability

How can we control generation results will be even more important in video generation than image generation. This study propose interesting approaches for controllability of video generation. The method proposed here allows user to specify object with bounding boxes, then set movement of boxes to control motion of the objects. It reminds ideas like DragGAN.

This study approaches to this with adding bounding box conditions to video diffusion model, then train model with dataset generated with tracking model to predict image and bounding boxes corresponds to the objects to improve tracking ability of the model. Then video is generated with bounding box inputs during inference time.

# Links

