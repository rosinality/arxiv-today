https://arxiv.org/abs/2503.11056

*Flow to the Mode: Mode-Seeking Diffusion Autoencoders for State-of-the-Art Image Tokenization* (Kyle Sargent, Kyle Hsu, Justin Johnson, Li Fei-Fei, Jiajun Wu)

> Since the advent of popular visual generation frameworks like VQGAN and latent diffusion models, state-of-the-art image generation systems have generally been two-stage systems that first tokenize or compress visual data into a lower-dimensional latent space before learning a generative model. Tokenizer training typically follows a standard recipe in which images are compressed and reconstructed subject to a combination of MSE, perceptual, and adversarial losses. Diffusion autoencoders have been proposed in prior work as a way to learn end-to-end perceptually-oriented image compression, but have not yet shown state-of-the-art performance on the competitive task of ImageNet-1K reconstruction. We propose FlowMo, a transformer-based diffusion autoencoder that achieves a new state-of-the-art for image tokenization at multiple compression rates without using convolutions, adversarial losses, spatially-aligned two-dimensional latent codes, or distilling from other tokenizers. Our key insight is that FlowMo training should be broken into a mode-matching pre-training stage and a mode-seeking post-training stage. In addition, we conduct extensive analyses and explore the training of generative models atop the FlowMo tokenizer. Our code and models will be available at http://kylesargent.github.io/flowmo .

Flow Matching 기반 이미지 토크나이저. 기본적인 인코더-디코더 학습 이후에 샘플링 과정에 대해 디코더를 학습시키는 절차가 추가됐네요.

<english>
Image tokenizer based on flow matching. After basic encoder-decoder training step for training decoder for sampling processes added.
</english>

#diffusion #tokenizer 