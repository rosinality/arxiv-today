https://arxiv.org/abs/2404.02905

*Visual Autoregressive Modeling: Scalable Image Generation via Next-Scale Prediction* (Keyu Tian, Yi Jiang, Zehuan Yuan, Bingyue Peng, Liwei Wang)

> We present Visual AutoRegressive modeling (VAR), a new generation paradigm that redefines the autoregressive learning on images as coarse-to-fine "next-scale prediction" or "next-resolution prediction", diverging from the standard raster-scan "next-token prediction". This simple, intuitive methodology allows autoregressive (AR) transformers to learn visual distributions fast and generalize well: VAR, for the first time, makes AR models surpass diffusion transformers in image generation. On ImageNet 256x256 benchmark, VAR significantly improve AR baseline by improving Frechet inception distance (FID) from 18.65 to 1.80, inception score (IS) from 80.4 to 356.4, with around 20x faster inference speed. It is also empirically verified that VAR outperforms the Diffusion Transformer (DiT) in multiple dimensions including image quality, inference speed, data efficiency, and scalability. Scaling up VAR models exhibits clear power-law scaling laws similar to those observed in LLMs, with linear correlation coefficients near -0.998 as solid evidence. VAR further showcases zero-shot generalization ability in downstream tasks including image in-painting, out-painting, and editing. These results suggest VAR has initially emulated the two important properties of LLMs: Scaling Laws and zero-shot task generalization. We have released all models and codes to promote the exploration of AR/VAR models for visual generation and unified learning.

이건 굉장히 흥미롭네요. VQVAE 기반으로 Autoregressive 생성을 하되 이전 토큰에 대해 Conditioning을 하는 것이 아니라 이전 스케일, 그러니까 좀 더 작은 스케일에서 나온 토큰들에 Conditioning을 해서 생성하는 방법입니다. 단순하면서도 흥미로운 결과가 나왔네요. VQ-VAE-2 (https://arxiv.org/abs/1906.00446) 의 Hierarchical한 시도가 다시 등장했다는 느낌도 있습니다.

Scaling Law를 추정한 결과도 나와있습니다. 어쩌면 이미지 생성 업계의 판도가 다시 한 번 뒤바뀔지도 모르겠군요.

#autoregressive-model #image-generation

# Links

[[200130 VQ-VAE-2.md]]