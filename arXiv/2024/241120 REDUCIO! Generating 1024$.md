https://arxiv.org/abs/2411.13552

*REDUCIO! Generating 1024$\times$1024 Video within 16 Seconds using Extremely Compressed Motion Latents* (Rui Tian, Qi Dai, Jianmin Bao, Kai Qiu, Yifan Yang, Chong Luo, Zuxuan Wu, Yu-Gang Jiang)

> Commercial video generation models have exhibited realistic, high-fidelity results but are still restricted to limited access. One crucial obstacle for large-scale applications is the expensive training and inference cost. In this paper, we argue that videos contain much more redundant information than images, thus can be encoded by very few motion latents based on a content image. Towards this goal, we design an image-conditioned VAE to encode a video to an extremely compressed motion latent space. This magic Reducio charm enables 64x reduction of latents compared to a common 2D VAE, without sacrificing the quality. Training diffusion models on such a compact representation easily allows for generating 1K resolution videos. We then adopt a two-stage video generation paradigm, which performs text-to-image and text-image-to-video sequentially. Extensive experiments show that our Reducio-DiT achieves strong performance in evaluation, though trained with limited GPU resources. More importantly, our method significantly boost the efficiency of video LDMs both in training and inference. We train Reducio-DiT in around 3.2K training hours in total and generate a 16-frame 1024*1024 video clip within 15.5 seconds on a single A100 GPU. Code released at https://github.com/microsoft/Reducio-VAE .

비디오 토크나이저를 3D 인코더 하나를 사용하는 대신 이미지 인코더와 3D 인코더의 조합으로 구성했군요. 이미지 정보가 주어진다면 움직임과 관련된 정보는 훨씬 고압축 하는 것이 가능하다는 아이디어죠.

<enligsh>
Design video tokenizer with combination of image encoder and 3d encoders, instead of using only 3d encoders. The main idea is that if we extract image informations, then we can compress more the information related with the motion.
</english>

#video-generation #tokenizer 