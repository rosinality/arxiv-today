https://ai.meta.com/static-resource/movie-gen-research-paper/

*Movie Gen: A Cast of Media Foundation Models* (The Movie Gen team @ Meta)

> We present Movie Gen, a cast of foundation models that generates high-quality, 1080p HD videos with different aspect ratios and synchronized audio. We also show additional capabilities such as precise instruction-based video editing and generation of personalized videos based on a user’s image. Our models set a new state-of-the-art on multiple tasks: text-to-video synthesis, video personalization, video editing, video-to-audio generation, and text-to-audio generation. Our largest video generation model is a 30B parameter transformer trained with a maximum context length of 73K video tokens, corresponding to a generated video of 16 seconds at 16 frames-per-second. We show multiple technical innovations and simplifications on the architecture, latent spaces, training objectives and recipes, data curation, evaluation protocols, parallelization techniques, and inference optimizations that allow us to reap the benefits of scaling pre-training data, model size, and training compute for training large scale media generation models. We hope this paper helps the research community to accelerate progress and innovation in media generation models.
> All videos from this paper are available at https://go.fb.me/MovieGenResearchVideos.

30B 16초, 16 fps Text-to-Image/Video 모델과 13B Video/Text-to-Audio 모델. VAE는 8x8x8 패치군요. 생성 백본에서는 2x Spatial Downsampling을 추가적으로 합니다. 텍스트 인코더로는 UL2, ByT5, MetaCLIP의 조합이고 7B Spatial Upsampler 사용. 그래서 대략 73K 토큰 입력이 되는군요.

H100 6000대 정도가 있다면 이런 모델을 학습시켜보는 것도 재미있을 것 같네요. 물론 데이터를 준비하는 것이 참 지난한 과정이었을 것 같긴 합니다만.

<english>
30B 16 second, 16 fps text-to-image/video model, and 13B video/text-to-audio model. They have used 8x8x8 patch VAE. Also, in generative backbones additional 2x spatial downsampling have been used. For text encoders combination of UL2, ByT5, MetaCLIP have used. And 7B spatial upsampler is applied. So they have used about 73K tokens for the video.

Maybe it is fun thing to train these kind of models if you have 6000 H100s. Of course preparing the data would be very hard and challenging.
</english>

#video-generation #flow-matching