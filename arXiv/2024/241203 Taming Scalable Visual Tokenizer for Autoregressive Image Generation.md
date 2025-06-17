https://arxiv.org/abs/2412.02692

*Taming Scalable Visual Tokenizer for Autoregressive Image Generation* (Fengyuan Shi, Zhuoyan Luo, Yixiao Ge, Yujiu Yang, Ying Shan, Limin Wang)

> Existing vector quantization (VQ) methods struggle with scalability, largely attributed to the instability of the codebook that undergoes partial updates during training. The codebook is prone to collapse as utilization decreases, due to the progressively widening distribution gap between non-activated codes and visual features. To solve the problem, we propose Index Backpropagation Quantization (IBQ), a new VQ method for the joint optimization of all codebook embeddings and the visual encoder. Applying a straight-through estimator on the one-hot categorical distribution between the encoded feature and codebook, all codes are differentiable and maintain a consistent latent space with the visual encoder. IBQ enables scalable training of visual tokenizers and, for the first time, achieves a large-scale codebook ($2^{18}$) with high dimension ($256$) and high utilization. Experiments on the standard ImageNet benchmark demonstrate the scalability and superiority of IBQ, achieving competitive results on both reconstruction ($1.00$ rFID) and autoregressive visual generation ($2.05$ gFID). The code and models are available at https://github.com/TencentARC/SEED-Voken.

VQ에서 선택된 코드만 업데이트 되기 때문에 업데이트 되지 않은 코드들과 인코더 출력의 괴리가 커지는 문제에 대한 해소. 얼마 전 나온 연구와 비슷한 문제의식입니다. (https://arxiv.org/abs/2411.02038) 여기에서는 Softmax의 그래디언트를 사용하는 방법을 사용했네요.

<english>
Resolving the problem of widening gap between non-updated codes and encoder features, which occurs because of VQ only updates selected codes. It is similar problem to a recent study (https://arxiv.org/abs/2411.02038). In this study they used a method of using the gradient of softmax.
</english>

#vq

# Links

[[241104 Addressing Representation Collapse in Vector Quantized Models with One Linear Layer.md]]