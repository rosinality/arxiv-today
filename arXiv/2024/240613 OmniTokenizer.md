https://arxiv.org/abs/2406.09399

*OmniTokenizer: A Joint Image-Video Tokenizer for Visual Generation* (Junke Wang, Yi Jiang, Zehuan Yuan, Binyue Peng, Zuxuan Wu, Yu-Gang Jiang)

> Tokenizer, serving as a translator to map the intricate visual data into a compact latent space, lies at the core of visual generative models. Based on the finding that existing tokenizers are tailored to image or video inputs, this paper presents OmniTokenizer, a transformer-based tokenizer for joint image and video tokenization. OmniTokenizer is designed with a spatial-temporal decoupled architecture, which integrates window and causal attention for spatial and temporal modeling. To exploit the complementary nature of image and video data, we further propose a progressive training strategy, where OmniTokenizer is first trained on image data on a fixed resolution to develop the spatial encoding capacity and then jointly trained on image and video data on multiple resolutions to learn the temporal dynamics. OmniTokenizer, for the first time, handles both image and video inputs within a unified framework and proves the possibility of realizing their synergy. Extensive experiments demonstrate that OmniTokenizer achieves state-of-the-art (SOTA) reconstruction performance on various image and video datasets, e.g., 1.11 reconstruction FID on ImageNet and 42 reconstruction FVD on UCF-101, beating the previous SOTA methods by 13% and 26%, respectively. Additionally, we also show that when integrated with OmniTokenizer, both language model-based approaches and diffusion models can realize advanced visual synthesis performance, underscoring the superiority and versatility of our method. Code is available at https://github.com/FoundationVision/OmniTokenizer.

이미지/비디오 토크나이저에 대한 관심이 다시 높아지고 있는 것 같네요. Spatio-Temporal 트랜스포머 인코더/디코더를 사용하고 이미지로 1단계, 비디오로 2단계 학습해서 이미지/비디오에 대한 토크나이저를 학습. 추가로 VQ 대신 VAE로 파인튜닝을 해보기도 했습니다.

그나저나 이제 Omni라는 단어가 인기를 얻겠군요.

#vq 