https://arxiv.org/abs/2403.05196

*Denoising Autoregressive Representation Learning* (Yazhe Li, Jorg Bornschein, Ting Chen)

> In this paper, we explore a new generative approach for learning visual representations. Our method, DARL, employs a decoder-only Transformer to predict image patches autoregressively. We find that training with Mean Squared Error (MSE) alone leads to strong representations. To enhance the image generation ability, we replace the MSE loss with the diffusion objective by using a denoising patch decoder. We show that the learned representation can be improved by using tailored noise schedules and longer training in larger models. Notably, the optimal schedule differs significantly from the typical ones used in standard image diffusion models. Overall, despite its simple architecture, DARL delivers performance remarkably close to state-of-the-art masked prediction models under the fine-tuning protocol. This marks an important step towards a unified model capable of both visual perception and generation, effectively combining the strengths of autoregressive and denoising diffusion models.

MSE를 사용한 패치 단위 Autoregressive 학습에 추가로 패치에 대한 Denoising Diffusion Objective를 결합해서 생성 능력의 개선을 시도했습니다. 인식 능력에 더해 생성 능력도 고려하고 싶고, 거기에 텍스트와의 결합까지 생각하자면 아키텍처적으로 탐색할 여지가 아직 많지 않나 싶습니다.

#pretraining #diffusion #autoregressive_model 