https://arxiv.org/abs/2402.13144

*Neural Network Diffusion* (Kai Wang, Zhaopan Xu, Yukun Zhou, Zelin Zang, Trevor Darrell, Zhuang Liu, Yang You)

> Diffusion models have achieved remarkable success in image and video generation. In this work, we demonstrate that diffusion models can also \textit{generate high-performing neural network parameters}. Our approach is simple, utilizing an autoencoder and a standard latent diffusion model. The autoencoder extracts latent representations of a subset of the trained network parameters. A diffusion model is then trained to synthesize these latent parameter representations from random noise. It then generates new representations that are passed through the autoencoder's decoder, whose outputs are ready to use as new subsets of network parameters. Across various architectures and datasets, our diffusion process consistently generates models of comparable or improved performance over trained networks, with minimal additional cost. Notably, we empirically find that the generated models perform differently with the trained networks. Our results encourage more exploration on the versatile use of diffusion models.

Latent Diffusion을 사용한 HyperNetwork? Weight의 일부를 Autoencoder로 Latent로 변환한 다음 Diffusion을 사용해 학습했습니다. 학습 샘플은 원 모델의 학습 과정의 마지막 Epoch에서 체크포인트를 여러 개 뽑아오는 방식으로 만들었군요. 아무래도 그냥 학습한 Weight를 그대로 복사하는 게 아니냐고 할 수 있어서 샘플링된 모델의 다양성으로 그에 대해 대답하고 있습니다.

#hypernetwork #diffusion 