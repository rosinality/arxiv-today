https://arxiv.org/abs/2403.13043

*When Do We Not Need Larger Vision Models?* (Baifeng Shi, Ziyang Wu, Maolin Mao, Xin Wang, Trevor Darrell)

> Scaling up the size of vision models has been the de facto standard to obtain more powerful visual representations. In this work, we discuss the point beyond which larger vision models are not necessary. First, we demonstrate the power of Scaling on Scales (S$^2$), whereby a pre-trained and frozen smaller vision model (e.g., ViT-B or ViT-L), run over multiple image scales, can outperform larger models (e.g., ViT-H or ViT-G) on classification, segmentation, depth estimation, Multimodal LLM (MLLM) benchmarks, and robotic manipulation. Notably, S$^2$ achieves state-of-the-art performance in detailed understanding of MLLM on the V* benchmark, surpassing models such as GPT-4V. We examine the conditions under which S$^2$ is a preferred scaling approach compared to scaling on model size. While larger models have the advantage of better generalization on hard examples, we show that features of larger vision models can be well approximated by those of multi-scale smaller models. This suggests most, if not all, of the representations learned by current large pre-trained models can also be obtained from multi-scale smaller models. Our results show that a multi-scale smaller model has comparable learning capacity to a larger model, and pre-training smaller models with S$^2$ can match or even exceed the advantage of larger models. We release a Python package that can apply S$^2$ on any vision model with one line of code: https://github.com/bfshi/scaling_on_scales.

ViT 인코더를 키우는 대신 입력 해상도를 키우면 어떨까? 에 대한 탐색. 요즘 자주 쓰이는 전체 이미지와 크롭에 대한 Feature를 결합하는 방식입니다. 여기서는 풀링을 써서 출력의 크기를 맞춰줬네요.

결론은 이미지 크기를 키우는 것이 모델을 키우는 것에 비해 잘 되는 경우가 많다는 것이네요. 롱테일 문제에서는 큰 모델이 강한데 이것도 고해상도 이미지에 대해 프리트레이닝을 하면 어느 정도 커버할 수 있다고 합니다.

사실 EfficientNet (https://arxiv.org/abs/1905.11946) 시절의 모델의 크기 뿐만 아니라 입력 해상도도 높여야 한다는 결론의 연장선상이지 않나 하는 생각을 합니다. 그리고 From Scratch 학습에 가까워질수록 이미지 인코더의 크기는 점점 덜 중요한 문제가 되지 않을까 싶습니다. 그렇지만 고해상도 이미지에 대응하는 것은 그 시점에서도 중요한 문제겠죠.

#vit #vision-language

# Links

