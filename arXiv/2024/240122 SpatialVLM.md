https://arxiv.org/abs/2401.12168

*SpatialVLM: Endowing Vision-Language Models with Spatial Reasoning Capabilities* (Boyuan Chen, Zhuo Xu, Sean Kirmani, Brian Ichter, Danny Driess, Pete Florence, Dorsa Sadigh, Leonidas Guibas, Fei Xia)

> Understanding and reasoning about spatial relationships is a fundamental capability for Visual Question Answering (VQA) and robotics. While Vision Language Models (VLM) have demonstrated remarkable performance in certain VQA benchmarks, they still lack capabilities in 3D spatial reasoning, such as recognizing quantitative relationships of physical objects like distances or size differences. We hypothesize that VLMs' limited spatial reasoning capability is due to the lack of 3D spatial knowledge in training data and aim to solve this problem by training VLMs with Internet-scale spatial reasoning data. To this end, we present a system to facilitate this approach. We first develop an automatic 3D spatial VQA data generation framework that scales up to 2 billion VQA examples on 10 million real-world images. We then investigate various factors in the training recipe, including data quality, training pipeline, and VLM architecture. Our work features the first internet-scale 3D spatial reasoning dataset in metric space. By training a VLM on such data, we significantly enhance its ability on both qualitative and quantitative spatial VQA. Finally, we demonstrate that this VLM unlocks novel downstream applications in chain-of-thought spatial reasoning and robotics due to its quantitative estimation capability. Project website: https://spatial-vlm.github.io/

VLM의 공간적 추론 능력을 향상시키기. Segmentation 등으로 객체들에 대한 정보를 뽑고 Depth Estimation으로 3D 정보를 추출한 다음 이 둘을 결합해 템플릿으로 VQA 데이터를 구축해서 학습하는 방법입니다. Vision-Language 데이터의 Recaptioning/Synthetic Data라는 흐름에서 3D에 대한 정보를 주입하는 것이라고 볼 수도 있겠네요.

데이터셋에서 더 많은 정보를 추출하기 위한 방법으로서의 Synthetic Data라는 것도 흥미로운 방향이라고 봅니다.

#vision-language #dataset #3d 