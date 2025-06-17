https://arxiv.org/abs/2410.05954

*Pyramidal Flow Matching for Efficient Video Generative Modeling* (Yang Jin, Zhicheng Sun, Ningyuan Li, Kun Xu, Kun Xu, Hao Jiang, Nan Zhuang, Quzhe Huang, Yang Song, Yadong Mu, Zhouchen Lin)

> Video generation requires modeling a vast spatiotemporal space, which demands significant computational resources and data usage. To reduce the complexity, the prevailing approaches employ a cascaded architecture to avoid direct training with full resolution. Despite reducing computational demands, the separate optimization of each sub-stage hinders knowledge sharing and sacrifices flexibility. This work introduces a unified pyramidal flow matching algorithm. It reinterprets the original denoising trajectory as a series of pyramid stages, where only the final stage operates at the full resolution, thereby enabling more efficient video generative modeling. Through our sophisticated design, the flows of different pyramid stages can be interlinked to maintain continuity. Moreover, we craft autoregressive video generation with a temporal pyramid to compress the full-resolution history. The entire framework can be optimized in an end-to-end manner and with a single unified Diffusion Transformer (DiT). Extensive experiments demonstrate that our method supports generating high-quality 5-second (up to 10-second) videos at 768p resolution and 24 FPS within 20.7k A100 GPU training hours. All code and models will be open-sourced at https://pyramid-flow.github.io.

비디오 생성 모델. 스케줄을 나눠서 대부분의 샘플링 과정을 저해상도에서 수행하게 하고, Autoregressive한 구조로 시간축에 대한 Conditioning을 하면서 과거일수록 저해상도의 정보를 사용하는 형태로 만들었군요.

<english>
Video generation model. Separate schedule and let most sampling is done at low resolution, and make it autoregressive which is conditioned on time axis, and use lower resolution information for more past frames.
</english>

#video-generation 