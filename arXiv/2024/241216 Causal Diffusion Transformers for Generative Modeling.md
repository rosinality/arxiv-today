https://arxiv.org/abs/2412.12095

*Causal Diffusion Transformers for Generative Modeling* (Chaorui Deng, Deyao Zh, Kunchang Li, Shi Guan, Haoqi Fan)

> We introduce Causal Diffusion as the autoregressive (AR) counterpart of Diffusion models. It is a next-token(s) forecasting framework that is friendly to both discrete and continuous modalities and compatible with existing next-token prediction models like LLaMA and GPT. While recent works attempt to combine diffusion with AR models, we show that introducing sequential factorization to a diffusion model can substantially improve its performance and enables a smooth transition between AR and diffusion generation modes. Hence, we propose CausalFusion - a decoder-only transformer that dual-factorizes data across sequential tokens and diffusion noise levels, leading to state-of-the-art results on the ImageNet generation benchmark while also enjoying the AR advantage of generating an arbitrary number of tokens for in-context reasoning. We further demonstrate CausalFusion's multimodal capabilities through a joint image generation and captioning model, and showcase CausalFusion's ability for zero-shot in-context image manipulations. We hope that this work could provide the community with a fresh perspective on training multimodal models over discrete and continuous data.

Autoregressive 모델과 Diffusion을 합치기. 이전의 깨끗한 토큰에 대해 다음 노이즈 토큰들에 대해 Diffusion을 하는 형태군요. MAR과 (https://arxiv.org/abs/2406.11838) Transfusion을 (https://arxiv.org/abs/2408.11039) 섞었다는 느낌입니다.

Continuous Token에 대한 Autoregression을 위해 Diffusion을 사용하는 것도 꽤 괜찮은 방향 같네요. (https://arxiv.org/abs/2412.08635)

<english>
Fusing autoregressive and diffusion. Conditioning on previous set of clear tokens doing diffusion on next noise tokens. It feels that this approach combines MAR (https://arxiv.org/abs/2406.11838)  and Transfusion (https://arxiv.org/abs/2408.11039).

I think it is quite promising research direction to use diffusion for autoregression on continuous tokens.
</english>

#autoregressive-model #diffusion #image-text

# Links

[[240617 Autoregressive Image Generation without Vector Quantization.md]]
[[241211 Multimodal Latent Language Modeling with Next-Token Diffusion.md]]
[[240820 Transfusion.md]]