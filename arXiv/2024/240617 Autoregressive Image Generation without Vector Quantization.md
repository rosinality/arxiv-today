https://arxiv.org/abs/2406.11838

*Autoregressive Image Generation without Vector Quantization* (Tianhong Li, Yonglong Tian, He Li, Mingyang Deng, Kaiming He)

> Conventional wisdom holds that autoregressive models for image generation are typically accompanied by vector-quantized tokens. We observe that while a discrete-valued space can facilitate representing a categorical distribution, it is not a necessity for autoregressive modeling. In this work, we propose to model the per-token probability distribution using a diffusion procedure, which allows us to apply autoregressive models in a continuous-valued space. Rather than using categorical cross-entropy loss, we define a Diffusion Loss function to model the per-token probability. This approach eliminates the need for discrete-valued tokenizers. We evaluate its effectiveness across a wide range of cases, including standard autoregressive models and generalized masked autoregressive (MAR) variants. By removing vector quantization, our image generator achieves strong results while enjoying the speed advantage of sequence modeling. We hope this work will motivate the use of autoregressive generation in other continuous-valued domains and applications.

Autoregressive 모델에서 Latent를 생성한 다음 이 Latent에 Conditional한 Diffusion Process를 사용해서 생성하는 모델. DARL과 비슷한 점이 있군요. (https://arxiv.org/abs/2403.05196) 추가적으로 Masked Image Modeling을 Mask 토큰을 예측하는 것을 반복하는 Autoregressive 모델로 보고 사용했습니다. VQ 대신 VAE와 연결할 수 있는 가능성 등에서 상당히 흥미롭네요.

#autoregressive-model #diffusion

# Links

[[240308 Denoising Autoregressive Representation Learning.md]]