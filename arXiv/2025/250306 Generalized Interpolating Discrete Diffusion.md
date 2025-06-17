https://arxiv.org/abs/2503.04482

*Generalized Interpolating Discrete Diffusion* (Dimitri von Rütte, Janis Fluri, Yuhui Ding, Antonio Orvieto, Bernhard Schölkopf, Thomas Hofmann)

> While state-of-the-art language models achieve impressive results through next-token prediction, they have inherent limitations such as the inability to revise already generated tokens. This has prompted exploration of alternative approaches such as discrete diffusion. However, masked diffusion, which has emerged as a popular choice due to its simplicity and effectiveness, reintroduces this inability to revise words. To overcome this, we generalize masked diffusion and derive the theoretical backbone of a family of general interpolating discrete diffusion (GIDD) processes offering greater flexibility in the design of the noising processes. Leveraging a novel diffusion ELBO, we achieve compute-matched state-of-the-art performance in diffusion language modeling. Exploiting GIDD's flexibility, we explore a hybrid approach combining masking and uniform noise, leading to improved sample quality and unlocking the ability for the model to correct its own mistakes, an area where autoregressive models notoriously have struggled. Our code and models are open-source: https://github.com/dvruette/gidd/

Discrete Diffusion 연구들이 많이 나오는 동시에 예측 토큰을 수정하지 못한다는 같은 문제를 태클하고 있네요. Discrete Diffusion을 확장해서 Masking 노이즈 뿐만 아니라 모든 단어에 대한 Uniform Probability 노이즈를 추가하는 방식이네요.

<english>
Research on discrete diffusion appears a lot recently, and they tackles problem of masked diffusion cannot replaces predicted tokens, simultaneously. They extended discrete diffusion and incorporates uniform probability noises on all vocabularies in addition to masking noises.
</english>

#diffusion #llm 