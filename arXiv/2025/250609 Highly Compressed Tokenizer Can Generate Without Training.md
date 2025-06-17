https://arxiv.org/abs/2506.08257

*Highly Compressed Tokenizer Can Generate Without Training* (L. Lao Beyer, T. Li, X. Chen, S. Karaman, K. He)

> Commonly used image tokenizers produce a 2D grid of spatially arranged tokens. In contrast, so-called 1D image tokenizers represent images as highly compressed one-dimensional sequences of as few as 32 discrete tokens. We find that the high degree of compression achieved by a 1D tokenizer with vector quantization enables image editing and generative capabilities through heuristic manipulation of tokens, demonstrating that even very crude manipulations -- such as copying and replacing tokens between latent representations of images -- enable fine-grained image editing by transferring appearance and semantic attributes. Motivated by the expressivity of the 1D tokenizer's latent space, we construct an image generation pipeline leveraging gradient-based test-time optimization of tokens with plug-and-play loss functions such as reconstruction or CLIP similarity. Our approach is demonstrated for inpainting and text-guided image editing use cases, and can generate diverse and realistic samples without requiring training of any generative model.

Semantic Tokenizer를 사용해 별도 생성 모델 없이 이미지 생성이나 편집이 가능하다는 연구. 이런 시도도 오랜만이네요.

<english>
A study that image generation or editing without generative models with semantic tokenizer.
</english>

#tokenizer #vq 