https://arxiv.org/abs/2403.06764

*An Image is Worth 1/2 Tokens After Layer 2: Plug-and-Play Inference Acceleration for Large Vision-Language Models* (Liang Chen, Haozhe Zhao, Tianyu Liu, Shuai Bai, Junyang Lin, Chang Zhou, Baobao Chang)

> In this study, we identify the inefficient attention phenomena in Large Vision-Language Models (LVLMs), notably within prominent models like LLaVA-1.5, QwenVL-Chat and Video-LLaVA. We find out that the attention computation over visual tokens is of extreme inefficiency in the deep layers of popular LVLMs, suggesting a need for a sparser approach compared to textual data handling. To this end, we introduce FastV, a versatile plug-and-play method designed to optimize computational efficiency by learning adaptive attention patterns in early layers and pruning visual tokens in subsequent ones. Our evaluations demonstrate FastV's ability to dramatically reduce computational costs (e.g., a 45 reduction in FLOPs for LLaVA-1.5-13B) without sacrificing performance in a wide range of image and video understanding tasks. The computational efficiency and performance trade-off of FastV are highly customizable and pareto-efficient. It can compress the FLOPs of a 13B-parameter model to achieve a lower budget than that of a 7B-parameter model, while still maintaining superior performance. We believe FastV has practical values for deployment of LVLMs in edge devices and commercial models. Code is released at https://github.com/pkunlp-icler/FastV.

이미지 토큰이 시퀀스 길이에 비해 실제로 주어지는 Attention 가중치는 적다는 결과. 즉 높은 단계의 레이어에서 이미지 토큰에는 Attention이 거의 주어지지 않고 다른 토큰에 이미지의 정보가 모두 흡수되는 것 같다고 주장합니다. 그러니 이런 이미지 토큰을 Pruning 하면 어떨까 하는 아이디어네요.

ViT에서 토큰을 Pruning하거나 Merging 하던 시도들이 생각나네요. (https://arxiv.org/abs/2210.09461)

이미지 시퀀스를 텍스트 시퀀스와 결합하는 것이 Long Context 측면과 잘 결합되는 감이 있어서 좋은 점이 있는 듯 한데 동시에 비효율성이 따라오는 것 같네요. Flamingo 스타일의 Cross Attention (https://arxiv.org/abs/2403.01487) 이 다시 나온 것도 그런 측면 때문이겠죠. 이 부분에서도 좋은 디자인을 할 수 있다면 재미있을 것 같네요.

#vision-language

# Links

[[240303 InfiMM-HD.md]]