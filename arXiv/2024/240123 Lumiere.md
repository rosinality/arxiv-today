https://arxiv.org/abs/2401.12945

*Lumiere: A Space-Time Diffusion Model for Video Generation* (Omer Bar-Tal, Hila Chefer, Omer Tov, Charles Herrmann, Roni Paiss, Shiran Zada, Ariel Ephrat, Junhwa Hur, Yuanzhen Li, Tomer Michaeli, Oliver Wang, Deqing Sun, Tali Dekel, Inbar Mosseri)

> We introduce Lumiere -- a text-to-video diffusion model designed for synthesizing videos that portray realistic, diverse and coherent motion -- a pivotal challenge in video synthesis. To this end, we introduce a Space-Time U-Net architecture that generates the entire temporal duration of the video at once, through a single pass in the model. This is in contrast to existing video models which synthesize distant keyframes followed by temporal super-resolution -- an approach that inherently makes global temporal consistency difficult to achieve. By deploying both spatial and (importantly) temporal down- and up-sampling and leveraging a pre-trained text-to-image diffusion model, our model learns to directly generate a full-frame-rate, low-resolution video by processing it in multiple space-time scales. We demonstrate state-of-the-art text-to-video generation results, and show that our design easily facilitates a wide range of content creation tasks and video editing applications, including image-to-video, video inpainting, and stylized generation.

https://lumiere-video.github.io/

구글의 비디오 생성 모형. Frame Interpolation/Temporal Super Resolution 없이 Space/Time에 대한 Downsampling을 하는 UNet으로 80 프레임(16 fps, 5초 분량)을 통째로 생성하는 모델을 만들고 그 위에 Sliding Window 방식으로 Spatial Super Resolution 모델을 올렸습니다.

#video-generation #diffusion 