https://arxiv.org/abs/2410.19324

*Simpler Diffusion (SiD2): 1.5 FID on ImageNet512 with pixel-space diffusion* (Emiel Hoogeboom, Thomas Mensink, Jonathan Heek, Kay Lamerigts, Ruiqi Gao, Tim Salimans)

> Latent diffusion models have become the popular choice for scaling up diffusion models for high resolution image synthesis. Compared to pixel-space models that are trained end-to-end, latent models are perceived to be more efficient and to produce higher image quality at high resolution. Here we challenge these notions, and show that pixel-space models can in fact be very competitive to latent approaches both in quality and efficiency, achieving 1.5 FID on ImageNet512 and new SOTA results on ImageNet128 and ImageNet256. We present a simple recipe for scaling end-to-end pixel-space diffusion models to high resolutions. 1: Use the sigmoid loss (Kingma & Gao, 2023) with our prescribed hyper-parameters. 2: Use our simplified memory-efficient architecture with fewer skip-connections. 3: Scale the model to favor processing the image at high resolution with fewer parameters, rather than using more parameters but at a lower resolution. When combining these three steps with recently proposed tricks like guidance intervals, we obtain a family of pixel-space diffusion models we call Simple Diffusion v2 (SiD2).

픽셀 단위 Diffusion. Loss Weighting을 Sigmoid로, 모델을 키우는 대신 패치 해상도를 증가시키기, 그리고 Residual Connection을 Downsampling 블록마다 하나로 줄이기.

<english>
Pixel level diffusion. Used sigmoid loss weighting, increase patch resolution instead of increasing model sizes, and reducing residual connections to once per each downsampling blocks.
</english>

#diffusion 