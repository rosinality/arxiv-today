https://arxiv.org/abs/2412.16326

*When Worse is Better: Navigating the compression-generation tradeoff in visual tokenization* (Vivek Ramanujan, Kushal Tirumala, Armen Aghajanyan, Luke Zettlemoyer, Ali Farhadi)

> Current image generation methods, such as latent diffusion and discrete token-based generation, depend on a two-stage training approach. In stage 1, an auto-encoder is trained to compress an image into a latent space; in stage 2, a generative model is trained to learn a distribution over that latent space. Most work focuses on maximizing stage 1 performance independent of stage 2, assuming better reconstruction always leads to better generation. However, we show this is not strictly true. Smaller stage 2 models can benefit from more compressed stage 1 latents even if reconstruction performance worsens, showing a fundamental trade-off between compression and generation modeling capacity. To better optimize this trade-off, we introduce Causally Regularized Tokenization (CRT), which uses knowledge of the stage 2 generation modeling procedure to embed useful inductive biases in stage 1 latents. This regularization makes stage 1 reconstruction performance worse, but makes stage 2 generation performance better by making the tokens easier to model: we are able to improve compute efficiency 2-3$\times$ over baseline and match state-of-the-art discrete autoregressive ImageNet generation (2.18 FID) with less than half the tokens per image (256 vs. 576) and a fourth the total model parameters (775M vs. 3.1B) as the previous SOTA (LlamaGen).

VQ와 Autoregressive 모델로 이루어진 이미지 생성 파이프라인에서 1단계 VQ의 성능이 높은 것이 더 나은 생성 결과로 이어지지 않는다는 문제에 대한 연구. Scaling Law를 기반으로 문제를 분석한 다음 VQ 단계에서 Autoregressive 모델을 붙여 Loss를 추가하는 형태로 이 트레이드오프에 대한 최적 지점을 찾으려고 시도했네요.

LLM 토크나이저도 그렇지만 Autoregressive 학습과는 별개로 학습되는 컴포넌트이기 때문에 문제가 발생할 수밖에 없죠. 이에 대한 한 가지 대응 방안은 최적 지점을 적절하게 선택하는 것인데, 늘 그렇지만 그런 문제에 대해서는 Scaling Law가 꾸준히 효과적이네요.

<english>
The research on the problem of better performance of first stage VQ in the image generation pipeline consist of VQ and autoregressive model does not transfer for better generation results. They analyzed the problem based on scaling law and tried to find optimal point of this trade-off by adding loss using autoregressive model in the VQ stage.

Like LLM tokenizers as VQ is separate component from autoregressive training it will constantly cause the problem. One solution for this is find out optimal point, and as always, scaling law is effective for these kind of problems.
</english>

#vq #autoregressive-model #scaling-law 