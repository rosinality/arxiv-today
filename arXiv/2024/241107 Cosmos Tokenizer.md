https://research.nvidia.com/labs/dir/cosmos-tokenizer/

*Cosmos Tokenizer: A suite of image and video neural tokenizers* (Fitsum Reda, Jinwei Gu, Xian Liu, Songwei Ge, Ting-Chun Wang, Haoxiang Wang, Ming-Yu Liu)

> We present Cosmos Tokenizer, a suite of image and video tokenizers that advances the state-of-the-art in visual tokenization, paving the way for scalable, robust and efficient development of large auto-regressive transformers (such as LLMs) or diffusion generators. This repo hosts the inference codes and shares pre-trained models for the different tokenizers. Please check out our [demo video](https://www.youtube.com/watch?v=Soy_myOfWIU).

NVIDIA의 이미지/비디오 토크나이저. 64K FSQ Discrete Token 혹은 KL 페널티 없는 바닐라 오토인코더를 사용한 Continuous Token. 비디오의 시간축에 대해서는 Causal합니다. CNN 기반으로 웨이블릿 공간에서 작동하는군요. Perceptual, Optical Flow, Gram Matrix Loss 사용까지. 굉장히 고전적인 맛의 모델이네요.

<english>
Image/Video tokenizer from NVIDIA. 64K FSQ discrete token or continuous token using vanilla autoencoder without KL penalty. It is causal along temporal axis of video. It is based on CNN and works on wavelet space. Perceptual, optical flow, gram matrix loss is used. Very classical taste model.
</english>

#tokenizer #vq