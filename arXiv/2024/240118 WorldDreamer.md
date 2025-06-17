https://arxiv.org/abs/2401.09985

*WorldDreamer: Towards General World Models for Video Generation via Predicting Masked Tokens* (Xiaofeng Wang, Zheng Zhu, Guan Huang, Boyuan Wang, Xinze Chen, Jiwen Lu)

> World models play a crucial role in understanding and predicting the dynamics of the world, which is essential for video generation. However, existing world models are confined to specific scenarios such as gaming or driving, limiting their ability to capture the complexity of general world dynamic environments. Therefore, we introduce WorldDreamer, a pioneering world model to foster a comprehensive comprehension of general world physics and motions, which significantly enhances the capabilities of video generation. Drawing inspiration from the success of large language models, WorldDreamer frames world modeling as an unsupervised visual sequence modeling challenge. This is achieved by mapping visual inputs to discrete tokens and predicting the masked ones. During this process, we incorporate multi-modal prompts to facilitate interaction within the world model. Our experiments show that WorldDreamer excels in generating videos across different scenarios, including natural scenes and driving environments. WorldDreamer showcases versatility in executing tasks such as text-to-video conversion, image-tovideo synthesis, and video editing. These results underscore WorldDreamer's effectiveness in capturing dynamic elements within diverse general world environments.

Masked Token Prediction + Spatiotemporal Patch에 대한 Local Attention Transformer 기반으로 비디오 생성 모델을 구성하고, 비디오 생성 모델에 다른 모달리티에 대한 Cross Attention을 붙인 형태의 모델. 따라서 이미지, 텍스트, 비디오, 그리고 운전 같은 액션을 컨디션으로 주는 것이 가능합니다.

아무래도 World Models라는 표현이 눈에 띌 수밖에 없네요. 비디오에 대한 학습이 세계에 대해 굉장히 강력한 정보를 줄 것이라는 가정이 많은데 실제로 그럴지가 앞으로 또 흥미로울 부분이 아닐까 싶습니다.

#video-generation #multimodal 