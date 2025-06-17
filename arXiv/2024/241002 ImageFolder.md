https://arxiv.org/abs/2410.01756

*ImageFolder: Autoregressive Image Generation with Folded Tokens* (Xiang Li, Hao Chen, Kai Qiu, Jason Kuen, Jiuxiang Gu, Bhiksha Raj, Zhe Lin)

> Image tokenizers are crucial for visual generative models, e.g., diffusion models (DMs) and autoregressive (AR) models, as they construct the latent representation for modeling. Increasing token length is a common approach to improve the image reconstruction quality. However, tokenizers with longer token lengths are not guaranteed to achieve better generation quality. There exists a trade-off between reconstruction and generation quality regarding token length. In this paper, we investigate the impact of token length on both image reconstruction and generation and provide a flexible solution to the tradeoff. We propose ImageFolder, a semantic tokenizer that provides spatially aligned image tokens that can be folded during autoregressive modeling to improve both generation efficiency and quality. To enhance the representative capability without increasing token length, we leverage dual-branch product quantization to capture different contexts of images. Specifically, semantic regularization is introduced in one branch to encourage compacted semantic information while another branch is designed to capture the remaining pixel-level details. Extensive experiments demonstrate the superior quality of image generation and shorter token length with ImageFolder tokenizer.

Autoregressive Image Generation을 가속하려면 토큰 시퀀스의 길이가 짧거나 혹은 여러 토큰을 한 번에 예측하는 것이 좋을 텐데, 토큰을 한 번에 예측하려면 토큰이 독립적인 쪽이 낫다는 아이디어군요. 그래서 디테일 토큰과 시맨틱 토큰을 분리해서 이 토큰의 결합을 통해 Reconstruction과 Generation을 한다는 아이디어입니다.

<english>
To accelerate autoregressive image generation it is preferred to have shorter sequences or predict multiple tokens at one time. To predict multiple tokens at the same time it is better to have independences on tokens. So this work tried to separate detail and semantic tokens, and do reconstruction and generation with concatenation of these 2 type of tokens.
</english>

#vq #autoregressive-model #image-generation 