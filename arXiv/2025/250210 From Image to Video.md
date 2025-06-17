https://arxiv.org/abs/2502.07001

*From Image to Video: An Empirical Study of Diffusion Representations* (Pedro Vélez, Luisa F. Polanía, Yi Yang, Chuhan Zhang, Rishab Kabra, Anurag Arnab, Mehdi S. M. Sajjadi)

> Diffusion models have revolutionized generative modeling, enabling unprecedented realism in image and video synthesis. This success has sparked interest in leveraging their representations for visual understanding tasks. While recent works have explored this potential for image generation, the visual understanding capabilities of video diffusion models remain largely uncharted. To address this gap, we systematically compare the same model architecture trained for video versus image generation, analyzing the performance of their latent representations on various downstream tasks including image classification, action recognition, depth estimation, and tracking. Results show that video diffusion models consistently outperform their image counterparts, though we find a striking range in the extent of this superiority. We further analyze features extracted from different layers and with varying noise levels, as well as the effect of model size and training budget on representation and generation quality. This work marks the first direct comparison of video and image diffusion objectives for visual understanding, offering insights into the role of temporal information in representation learning.

비디오 생성으로 학습된 Diffusion이 이미지 생성으로 학습된 모델보다 더 나은 Feature Extractor였다는 연구. 어쩌면 비디오 생성까지 탑재된 모델이 멀티모달 모델의 방향이 되어야 할지도 모르겠네요.

<english>
The study insist that diffusion trained on video generation is better feature extractor then trained on image generation. Maybe future direction of multimodal model should incorporate video generation.
</english>

#video-generation #diffusion #image-generation 