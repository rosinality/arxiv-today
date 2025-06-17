https://arxiv.org/abs/2506.08010

*Vision Transformers Don't Need Trained Registers* (Nick Jiang, Amil Dravid, Alexei Efros, Yossi Gandelsman)

> We investigate the mechanism underlying a previously identified phenomenon in Vision Transformers -- the emergence of high-norm tokens that lead to noisy attention maps. We observe that in multiple models (e.g., CLIP, DINOv2), a sparse set of neurons is responsible for concentrating high-norm activations on outlier tokens, leading to irregular attention patterns and degrading downstream visual processing. While the existing solution for removing these outliers involves retraining models from scratch with additional learned register tokens, we use our findings to create a training-free approach to mitigate these artifacts. By shifting the high-norm activations from our discovered register neurons into an additional untrained token, we can mimic the effect of register tokens on a model already trained without registers. We demonstrate that our method produces cleaner attention and feature maps, enhances performance over base models across multiple downstream visual tasks, and achieves results comparable to models explicitly trained with register tokens. We then extend test-time registers to off-the-shelf vision-language models to improve their interpretability. Our results suggest that test-time registers effectively take on the role of register tokens at test-time, offering a training-free solution for any pre-trained model released without them.

ViT의 아웃라이어 토큰을 임의의 위치로 이동시키는 방법을 연구했군요. 아예 이미지 밖으로 제외시키면 레지스터 토큰처럼 기능하게 된다고.

<english>
A study on moving outlier tokens from ViT to arbitrary positions. If it is moved to the outside of the image then it works as register tokens.
</english>

#vit #transformer 