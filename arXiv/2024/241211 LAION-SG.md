https://arxiv.org/abs/2412.08580

*LAION-SG: An Enhanced Large-Scale Dataset for Training Complex Image-Text Models with Structural Annotations* (Zejian Li, Chenye Meng, Yize Li, Ling Yang, Shengyuan Zhang, Jiarui Ma, Jiayi Li, Guang Yang, Changyuan Yang, Zhiyuan Yang, Jinxiong Chang, Lingyun Sun)

> Recent advances in text-to-image (T2I) generation have shown remarkable success in producing high-quality images from text. However, existing T2I models show decayed performance in compositional image generation involving multiple objects and intricate relationships. We attribute this problem to limitations in existing datasets of image-text pairs, which lack precise inter-object relationship annotations with prompts only. To address this problem, we construct LAION-SG, a large-scale dataset with high-quality structural annotations of scene graphs (SG), which precisely describe attributes and relationships of multiple objects, effectively representing the semantic structure in complex scenes. Based on LAION-SG, we train a new foundation model SDXL-SG to incorporate structural annotation information into the generation process. Extensive experiments show advanced models trained on our LAION-SG boast significant performance improvements in complex scene generation over models on existing datasets. We also introduce CompSG-Bench, a benchmark that evaluates models on compositional image generation, establishing a new standard for this domain.

Text to Image 모델에서 여러 객체들과 그 관계를 제대로 이미지에 반영하지 못하는 문제를 해소하기 위해 Scene Graph 데이터셋을 생성하고, Scene Graph를 입력으로 받는 모델을 디자인. 최근에 Scene Graph를 사용해 Instruction 데이터를 구축하는 시도도 있었죠. (https://arxiv.org/abs/2412.07012) Scene Graph를 잘 만드는 것이 문제이긴 하지만 흥미로운 시도가 아닌가 싶습니다.

<english>
To resolve the problem of text to image models cannot reflect well multiple objects and its relationships into the image, this study generated scene graph dataset, and designed the model that accepts scene graph inputs. Recently there was an approach to construct instruction data using scene graph. (https://arxiv.org/abs/2412.07012) Though build scene graph well itself will be a problem, but I think this is interesting approach.
</english>

#text-to-image #synthetic-data

# Links

