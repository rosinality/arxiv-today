https://arxiv.org/abs/2502.20586

*Training LLMs with MXFP4* (Albert Tseng, Tao Yu, Youngsuk Park)

> Low precision (LP) datatypes such as MXFP4 can accelerate matrix multiplications (GEMMs) and reduce training costs. However, directly using MXFP4 instead of BF16 during training significantly degrades model quality. In this work, we present the first near-lossless training recipe that uses MXFP4 GEMMs, which are $2\times$ faster than FP8 on supported hardware. Our key insight is to compute unbiased gradient estimates with stochastic rounding (SR), resulting in more accurate model updates. However, directly applying SR to MXFP4 can result in high variance from block-level outliers, harming convergence. To overcome this, we use the random Hadamard tranform to theoretically bound the variance of SR. We train GPT models up to 6.7B parameters and find that our method induces minimal degradation over mixed-precision BF16 training. Our recipe computes $>1/2$ the training FLOPs in MXFP4, enabling an estimated speedup of $>1.3\times$ over FP8 and $>1.7\times$ over BF16 during backpropagation.

MXFP4를 통한 학습 연구가 나오기 시작하네요. (https://arxiv.org/abs/2502.20853) 학습용으로는 MXFP6도 관심이 높은 것 같습니다. 물론 지속적으로 MXFP4 학습에 도전한 사례가 나올 것 같지만요.

<english>
The research on training with MXFP4 is starts to appearing (https://arxiv.org/abs/2502.20853). For training MXFP6 is also gaining traction. But of course there would be continual trial to challenge on MXFP4 training.
</english>

#quantization #efficient-training 