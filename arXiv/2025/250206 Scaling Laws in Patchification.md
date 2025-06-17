https://arxiv.org/abs/2502.03738

*Scaling Laws in Patchification: An Image Is Worth 50,176 Tokens And More* (Feng Wang, Yaodong Yu, Guoyizhe Wei, Wei Shao, Yuyin Zhou, Alan Yuille, Cihang Xie)

> Since the introduction of Vision Transformer (ViT), patchification has long been regarded as a de facto image tokenization approach for plain visual architectures. By compressing the spatial size of images, this approach can effectively shorten the token sequence and reduce the computational cost of ViT-like plain architectures. In this work, we aim to thoroughly examine the information loss caused by this patchification-based compressive encoding paradigm and how it affects visual understanding. We conduct extensive patch size scaling experiments and excitedly observe an intriguing scaling law in patchification: the models can consistently benefit from decreased patch sizes and attain improved predictive performance, until it reaches the minimum patch size of 1x1, i.e., pixel tokenization. This conclusion is broadly applicable across different vision tasks, various input scales, and diverse architectures such as ViT and the recent Mamba models. Moreover, as a by-product, we discover that with smaller patches, task-specific decoder heads become less critical for dense prediction. In the experiments, we successfully scale up the visual sequence to an exceptional length of 50,176 tokens, achieving a competitive test accuracy of 84.6% with a base-sized model on the ImageNet-1k benchmark. We hope this study can provide insights and theoretical foundations for future works of building non-compressive vision models. Code is available at https://github.com/wangf3014/Patch_Scaling.

패치 크기에 대한 Scaling Law. 기본적으로 패치 크기가 작을수록 더 고성능입니다. 다만 최적점을 찾고자 한다면 해상도와 패치 크기, 모델 크기, Vision Language 모델이라면 LLM의 크기까지 같이 고려해야 하겠죠.

<english>
Scaling law for patch sizes. By default, smaller patch sizes lead to better performance. But if we want to find optimal points then we should account resolutions, patch sizes, model sizes, and for vision-language models, size of LLMs.
</english>

#scaling-law #vit 