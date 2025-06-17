https://arxiv.org/abs/2403.01487

*InfiMM-HD: A Leap Forward in High-Resolution Multimodal Understanding* (Haogeng Liu, Quanzeng You, Xiaotian Han, Yiqi Wang, Bohan Zhai, Yongfei Liu, Yunzhe Tao, Huaibo Huang, Ran He, Hongxia Yang)

> Multimodal Large Language Models (MLLMs) have experienced significant advancements recently. Nevertheless, challenges persist in the accurate recognition and comprehension of intricate details within high-resolution images. Despite being indispensable for the development of robust MLLMs, this area remains underinvestigated. To tackle this challenge, our work introduces InfiMM-HD, a novel architecture specifically designed for processing images of different resolutions with low computational overhead. This innovation facilitates the enlargement of MLLMs to higher-resolution capabilities. InfiMM-HD incorporates a cross-attention module and visual windows to reduce computation costs. By integrating this architectural design with a four-stage training pipeline, our model attains improved visual perception efficiently and cost-effectively. Empirical study underscores the robustness and effectiveness of InfiMM-HD, opening new avenues for exploration in related areas. Codes and models can be found at https://huggingface.co/Infi-MM/infimm-hd

고해상도 VLM. Flamingo 스타일의 Cross Attention 기반 모델을 채택했군요. 테스트해봤더니 Cross Attention은 4개 블럭 당 하나면 충분한 것 같고 따라서 시퀀스에 그대로 붙이는 것보다 이미지 토큰이 많아지는 경우에 더 효율적일 수 있다는 아이디어입니다.

224px로 시작한 다음 448px로 썸네일과 크롭을 붙여 사용하는 세팅을 사용했습니다.

#vision-language 