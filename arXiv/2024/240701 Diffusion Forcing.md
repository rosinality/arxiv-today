https://arxiv.org/abs/2407.01392

*Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion* (Boyuan Chen, Diego Marti Monso, Yilun Du, Max Simchowitz, Russ Tedrake, Vincent Sitzmann)

> This paper presents Diffusion Forcing, a new training paradigm where a diffusion model is trained to denoise a set of tokens with independent per-token noise levels. We apply Diffusion Forcing to sequence generative modeling by training a causal next-token prediction model to generate one or several future tokens without fully diffusing past ones. Our approach is shown to combine the strengths of next-token prediction models, such as variable-length generation, with the strengths of full-sequence diffusion models, such as the ability to guide sampling to desirable trajectories. Our method offers a range of additional capabilities, such as (1) rolling-out sequences of continuous tokens, such as video, with lengths past the training horizon, where baselines diverge and (2) new sampling and guiding schemes that uniquely profit from Diffusion Forcing's variable-horizon and causal architecture, and which lead to marked performance gains in decision-making and planning tasks. In addition to its empirical success, our method is proven to optimize a variational lower bound on the likelihoods of all subsequences of tokens drawn from the true joint distribution. Project website: https://boyuan.space/diffusion-forcing/

Diffusion과 Autoregressive 모델의 결합으로 두 모델이 장점을 합칠 수 있다는 아이디어. 여기서의 특징은 한 시퀀스 내의 각 토큰마다 서로 다른 노이즈 레벨을 적용했다는 것이네요.

Autoregressive 모델을 통해 많은 모달리티를 통합하고 싶은 시점에서 Diffusion Loss를 사용해 Autoregressive 모델의 한계를 커버하는 것은 흥미로운 접근인 것 같습니다. (https://arxiv.org/abs/2403.05196, https://arxiv.org/abs/2406.11838)

#diffusion #autoregressive-model

# Links

[[240617 Autoregressive Image Generation without Vector Quantization.md]]
[[240308 Denoising Autoregressive Representation Learning.md]]