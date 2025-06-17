https://arxiv.org/abs/2503.00307

*Remasking Discrete Diffusion Models with Inference-Time Scaling* (Guanghan Wang, Yair Schiff, Subham Sekhar Sahoo, Volodymyr Kuleshov)

> Part of the success of diffusion models stems from their ability to perform iterative refinement, i.e., repeatedly correcting outputs during generation. However, modern masked discrete diffusion lacks this capability: when a token is generated, it cannot be updated again, even when it introduces an error. Here, we address this limitation by introducing the remasking diffusion model (ReMDM) sampler, a method that can be applied to pretrained masked diffusion models in a principled way and that is derived from a discrete diffusion model with a custom remasking backward process. Most interestingly, ReMDM endows discrete diffusion with a form of inference-time compute scaling. By increasing the number of sampling steps, ReMDM generates natural language outputs that approach the quality of autoregressive models, whereas when the computation budget is limited, ReMDM better maintains quality. ReMDM also improves sample quality of masked diffusion models for discretized images, and in scientific domains such as molecule design, ReMDM facilitates diffusion guidance and pushes the Pareto frontier of controllability relative to classical masking and uniform noise diffusion. We provide the code along with a blog post on the project page: https://remdm.github.io.

요즘 Diffusion LM이 다시 등장하고 있네요. (https://www.inceptionlabs.ai/) Diffusion LM의 샘플링 과정에서 예측된 토큰을 다시 마스킹할 수는 없다는 문제를 해소하려 시도했습니다. LLaDA에서도 (https://arxiv.org/abs/2502.09992) Remasking 전략을 사용했었죠.

<english>
Recently diffusion LM appears again (https://www.inceptionlabs.ai/). They tried to resolve it cannot remask tokens predicted during sampling process of diffusion LM. LLaDA (https://arxiv.org/abs/2502.09992) also adopted remasking strategy.
</english>

#diffusion #llm 