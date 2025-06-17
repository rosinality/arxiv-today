https://arxiv.org/abs/2310.19909

Battle of the Backbones: A Large-Scale Comparison of Pretrained Models across Computer Vision Tasks (Micah Goldblum, Hossein Souri, Renkun Ni, Manli Shu, Viraj Prabhu, Gowthami Somepalli, Prithvijit Chattopadhyay, Mark Ibrahim, Adrien Bardes, Judy Hoffman, Rama Chellappa, Andrew Gordon Wilson, Tom Goldstein)

이미지 백본에 대한 다양한 과제에 대한 퍼포먼스 비교입니다. 이미지 분류 같은 프리트레이닝은 모든 아키텍처에 대해서 했지만 다른 프리트레이닝 방법은 특정 아키텍처에 대해서만 되어 있다거나, 이미지넷 1K에 대한 프리트레이닝 결과만 있다거나 하는 등의 특징이 있어서 좀 자세히 봐야할 것 같군요.

그래도 논문에서 발견한 것들을 정리해보면 이렇습니다.

1. 이미지넷 21K에 대해 supervised pretraining한 ConvNeXt가 가장 강력. Swin이 ViT보다 나음.
2. ViT가 CNN보다 scaling이 더 잘 되는 듯.
3. supervised가 나은가 self supervised가 나은가? 학습 데이터셋 크기가 달라서 비교하기 어렵지만 분류나 retrieval에는 SSL이 나은 것 같기도. 그런데 supervised training이 detection과 segmentation에서는 스코어가 더 잘 나오는 듯.
4. 과제들의 성능은 상관관계가 높음.
5. ViT는 linear probing보다 파인튜닝의 수혜를 봄.
6. ViT 중에서는 CLIP이 가장 강력.
7. MAE나 Diffusion보다는 supervised 혹은 contrastive learning이 더 나았음.

#backbone #vit #cnn 

[[231025 ConvNets Match Vision Transformers at Scale]]