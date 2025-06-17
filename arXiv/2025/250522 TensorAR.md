https://arxiv.org/abs/2505.16324

*TensorAR: Refinement is All You Need in Autoregressive Image Generation* (Cheng Cheng, Lin Song, Yicheng Xiao, Yuxin Chen, Xuchong Zhang, Hongbin Sun, Ying Shan)

> Autoregressive (AR) image generators offer a language-model-friendly approach to image generation by predicting discrete image tokens in a causal sequence. However, unlike diffusion models, AR models lack a mechanism to refine previous predictions, limiting their generation quality. In this paper, we introduce TensorAR, a new AR paradigm that reformulates image generation from next-token prediction to next-tensor prediction. By generating overlapping windows of image patches (tensors) in a sliding fashion, TensorAR enables iterative refinement of previously generated content. To prevent information leakage during training, we propose a discrete tensor noising scheme, which perturbs input tokens via codebook-indexed noise. TensorAR is implemented as a plug-and-play module compatible with existing AR models. Extensive experiments on LlamaGEN, Open-MAGVIT2, and RAR demonstrate that TensorAR significantly improves the generation performance of autoregressive models.

AR 이미지 생성에서 다중 토큰 입력/출력을 적용. 이후에 예측한 토큰으로 이전에 예측한 토큰을 보정할 수 있다는 아이디어. 이대로는 입력을 그대로 복사하면 그만이기 때문에 노이즈를 추가합니다.

<english>
Applying multiple token input and output for AR image generation. The idea is we can revise predicted token using tokens predicted later. As it became trivial objective by just copying the inputs, noise is added to the input.
</english>

#autoregressive-model #image-generation 