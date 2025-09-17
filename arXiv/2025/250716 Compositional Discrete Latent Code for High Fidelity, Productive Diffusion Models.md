https://arxiv.org/abs/2507.12318

*Compositional Discrete Latent Code for High Fidelity, Productive Diffusion Models* (Samuel Lavoie, Michael Noukhovitch, Aaron Courville)

> We argue that diffusion models' success in modeling complex distributions is, for the most part, coming from their input conditioning. This paper investigates the representation used to condition diffusion models from the perspective that ideal representations should improve sample fidelity, be easy to generate, and be compositional to allow out-of-training samples generation. We introduce Discrete Latent Code (DLC), an image representation derived from Simplicial Embeddings trained with a self-supervised learning objective. DLCs are sequences of discrete tokens, as opposed to the standard continuous image embeddings. They are easy to generate and their compositionality enables sampling of novel images beyond the training distribution. Diffusion models trained with DLCs have improved generation fidelity, establishing a new state-of-the-art for unconditional image generation on ImageNet. Additionally, we show that composing DLCs allows the image generator to produce out-of-distribution samples that coherently combine the semantics of images in diverse ways. Finally, we showcase how DLCs can enable text-to-image generation by leveraging large-scale pretrained language models. We efficiently finetune a text diffusion language model to generate DLCs that produce novel samples outside of the image generator training distribution.

Discrete Latent Code를 Condition으로 사용해 Diffusion 모델 학습을 개선할 수 있다는 아이디어. 더 나아가 Compositional Generalization을 촉진한다고. Continuous Code로는 안 되는가 하는 질문에 대해서는 Continuous한 쪽이 학습이 더 어렵다고 하는군요.

<english>
Idea of improving diffusion model training by using discrete latent code as a condition. Furthermore, it could enhance compositional generalization. We can naturally asks about continuous codes, and the authors insist that it is harder to train with continuous codes.

#diffusion 