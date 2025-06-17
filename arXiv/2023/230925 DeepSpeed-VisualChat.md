https://arxiv.org/abs/2309.14327

DeepSpeed-VisualChat: Multi-Round Multi-Image Interleave Chat via Multi-Modal Causal Attention (Zhewei Yao, Xiaoxia Wu, Conglong Li, Minjia Zhang, Heyang Qi, Olatunji Ruwase, Ammar Ahmad Awan, Samyam Rajbhandari, Yuxiong He)

DeepSpeed에서 Image-Text 채팅을 위한 모델 프레임워크를 만들었군요. 전반적인 구조는 이미지 토큰을 텍스트 토큰과 결합하는 일반적인(?) 형태인데, 이미지 토큰은 이미지 인코더를 거쳐왔으니 토큰 사이 Attention이 필요하지 않다, 텍스트와 이미지 토큰에 대한 Attention은 분리되어야 한다는 제안을 하고 있군요. 어느 정도의 효과인지는 나와있지 않지만요.

#vision-language #multimodal 