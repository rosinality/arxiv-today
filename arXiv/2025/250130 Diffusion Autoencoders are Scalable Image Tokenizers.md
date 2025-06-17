https://arxiv.org/abs/2501.18593

*Diffusion Autoencoders are Scalable Image Tokenizers* (Yinbo Chen, Rohit Girdhar, Xiaolong Wang, Sai Saketh Rambhatla, Ishan Misra)

> Tokenizing images into compact visual representations is a key step in learning efficient and high-quality image generative models. We present a simple diffusion tokenizer (DiTo) that learns compact visual representations for image generation models. Our key insight is that a single learning objective, diffusion L2 loss, can be used for training scalable image tokenizers. Since diffusion is already widely used for image generation, our insight greatly simplifies training such tokenizers. In contrast, current state-of-the-art tokenizers rely on an empirically found combination of heuristics and losses, thus requiring a complex training recipe that relies on non-trivially balancing different losses and pretrained supervised models. We show design decisions, along with theoretical grounding, that enable us to scale DiTo for learning competitive image representations. Our results show that DiTo is a simpler, scalable, and self-supervised alternative to the current state-of-the-art image tokenizer which is supervised. DiTo achieves competitive or better quality than state-of-the-art in image reconstruction and downstream image generation tasks.

Flow Matching으로 학습한 인코더의 출력을 이미지 토큰으로 사용하는 방법. 굉장히 흥미롭네요. Diffusion이 이미지 인코더로서도 기능할 수 있다는 연구를 고려할 때 최근 제안되는 문제들인 이미지 토큰에 Semantic한 정보가 부족한 문제도 해소될 수 있지 않을까 싶습니다.

The method of using the output of an encoder trained with flow matching as image tokens. It is very interesting. Considering studies that show diffusion can be used as an image encoder, I think this could help resolve recent issues about image tokens are lacking semantic information.

#diffusion #tokenizer #image-generation 