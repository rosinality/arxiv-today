https://arxiv.org/abs/2501.10064

*One-D-Piece: Image Tokenizer Meets Quality-Controllable Compression* (Keita Miwa, Kento Sasaki, Hidehisa Arai, Tsubasa Takahashi, Yu Yamaguchi)

> Current image tokenization methods require a large number of tokens to capture the information contained within images. Although the amount of information varies across images, most image tokenizers only support fixed-length tokenization, leading to inefficiency in token allocation. In this study, we introduce One-D-Piece, a discrete image tokenizer designed for variable-length tokenization, achieving quality-controllable mechanism. To enable variable compression rate, we introduce a simple but effective regularization mechanism named "Tail Token Drop" into discrete one-dimensional image tokenizers. This method encourages critical information to concentrate at the head of the token sequence, enabling support of variadic tokenization, while preserving state-of-the-art reconstruction quality. We evaluate our tokenizer across multiple reconstruction quality metrics and find that it delivers significantly better perceptual quality than existing quality-controllable compression methods, including JPEG and WebP, at smaller byte sizes. Furthermore, we assess our tokenizer on various downstream computer vision tasks, including image classification, object detection, semantic segmentation, and depth estimation, confirming its adaptability to numerous applications compared to other variable-rate methods. Our approach demonstrates the versatility of variable-length discrete image tokenization, establishing a new paradigm in both compression efficiency and reconstruction performance. Finally, we validate the effectiveness of tail token drop via detailed analysis of tokenizers.

가변 길이 이미지 토크나이저. Semantic Tokenizer 위에 학습 시 일부 토큰을 Drop하는 방법을 사용했습니다. Matryoshka Embedding 같이 생각할 수 있겠네요.

<english>
Image tokenizer with varying token length. Method is based on partially droppping the tokens during training with semantic tokenizers. It maybe thought as similar approach to Matryoshka Embedding.
</english>

#tokenizer #image-generation 