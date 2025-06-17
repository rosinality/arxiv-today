https://arxiv.org/abs/2502.13967

*FlexTok: Resampling Images into 1D Token Sequences of Flexible Length* (Roman Bachmann, Jesse Allardice, David Mizrahi, Enrico Fini, Oğuzhan Fatih Kar, Elmira Amirloo, Alaaeldin El-Nouby, Amir Zamir, Afshin Dehghan)

> Image tokenization has enabled major advances in autoregressive image generation by providing compressed, discrete representations that are more efficient to process than raw pixels. While traditional approaches use 2D grid tokenization, recent methods like TiTok have shown that 1D tokenization can achieve high generation quality by eliminating grid redundancies. However, these methods typically use a fixed number of tokens and thus cannot adapt to an image's inherent complexity. We introduce FlexTok, a tokenizer that projects 2D images into variable-length, ordered 1D token sequences. For example, a 256x256 image can be resampled into anywhere from 1 to 256 discrete tokens, hierarchically and semantically compressing its information. By training a rectified flow model as the decoder and using nested dropout, FlexTok produces plausible reconstructions regardless of the chosen token sequence length. We evaluate our approach in an autoregressive generation setting using a simple GPT-style Transformer. On ImageNet, this approach achieves an FID<2 across 8 to 128 tokens, outperforming TiTok and matching state-of-the-art methods with far fewer tokens. We further extend the model to support to text-conditioned image generation and examine how FlexTok relates to traditional 2D tokenization. A key finding is that FlexTok enables next-token prediction to describe images in a coarse-to-fine "visual vocabulary", and that the number of tokens to generate depends on the complexity of the generation task.

가변 길이 Semantic Tokenizer가 나왔네요. (https://arxiv.org/abs/2501.10064) 토크나이저의 디코더로는 Rectified Flow를 사용했군요.

개인적으로 Semantic Tokenizer는 Token Pruning이나 Resampling과 비슷한 접근이라는 생각이 있습니다. 고해상도 이미지로 넘어갔을 때, 그리고 인식에서도 Scalable한 방법일지 궁금하긴 하네요.

<english>
Variant length semantic image tokenizer (https://arxiv.org/abs/2501.10064). They used rectified flow as a decoder of tokenizer.

I suspect semantic tokenizer is similar approach to token pruning or resampling. I wonder it would be scalable for high resolution images and image recognitions.
</english>

#vq #diffusion #autoregressive-model 