https://arxiv.org/abs/2507.15856

*Latent Denoising Makes Good Visual Tokenizers* (Jiawei Yang, Tianhong Li, Lijie Fan, Yonglong Tian, Yue Wang)

> Despite their fundamental role, it remains unclear what properties could make visual tokenizers more effective for generative modeling. We observe that modern generative models share a conceptually similar training objective -- reconstructing clean signals from corrupted inputs such as Gaussian noise or masking -- a process we term denoising. Motivated by this insight, we propose aligning tokenizer embeddings directly with the downstream denoising objective, encouraging latent embeddings to be more easily reconstructed even when heavily corrupted. To achieve this, we introduce the Latent Denoising Tokenizer (l-DeTok), a simple yet effective tokenizer trained to reconstruct clean images from latent embeddings corrupted by interpolative noise and random masking. Extensive experiments on ImageNet 256x256 demonstrate that our tokenizer consistently outperforms standard tokenizers across six representative generative models. Our findings highlight denoising as a fundamental design principle for tokenizer development, and we hope it could motivate new perspectives for future tokenizer design.

이미지 토크나이저를 디노이징으로 학습시키면 이후 디노이징 모델에 사용하기 적합할 것이라는 아이디어. 디노이징 과제의 난점을 토크나이저로 옮긴 것이 아닌가 싶기도.

If we train an image tokenizer with denoising, it could be better for downstream denoising tasks. I wonder if this shifts the burden of denoising tasks to the tokenizers.

#tokenizer 