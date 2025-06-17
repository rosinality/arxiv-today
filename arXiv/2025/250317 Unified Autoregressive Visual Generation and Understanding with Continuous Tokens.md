https://arxiv.org/abs/2503.13436

*Unified Autoregressive Visual Generation and Understanding with Continuous Tokens* (Lijie Fan, Luming Tang, Siyang Qin, Tianhong Li, Xuan Yang, Siyuan Qiao, Andreas Steiner, Chen Sun, Yuanzhen Li, Tao Zhu, Michael Rubinstein, Michalis Raptis, Deqing Sun, Radu Soricut)

> We present UniFluid, a unified autoregressive framework for joint visual generation and understanding leveraging continuous visual tokens. Our unified autoregressive architecture processes multimodal image and text inputs, generating discrete tokens for text and continuous tokens for image. We find though there is an inherent trade-off between the image generation and understanding task, a carefully tuned training recipe enables them to improve each other. By selecting an appropriate loss balance weight, the unified model achieves results comparable to or exceeding those of single-task baselines on both tasks. Furthermore, we demonstrate that employing stronger pre-trained LLMs and random-order generation during training is important to achieve high-fidelity image generation within this unified framework. Built upon the Gemma model series, UniFluid exhibits competitive performance across both image generation and understanding, demonstrating strong transferability to various downstream tasks, including image editing for generation, as well as visual captioning and question answering for understanding.

이미지 생성과 인식을 통합하는 모델인데 Janus처럼 (https://arxiv.org/abs/2410.13848) 인식과 생성을 위한 이미지 인코더를 분리했군요. 생성엔 Diffusion Head를 사용하네요.

<english>
Unified image understanding and generation model, with separate encoder for understanding and generation, like Janus (https://arxiv.org/abs/2410.13848). Diffusion head is used for generation.
</english>

#image-generation #image-understanding #autoregressive-model #diffusion 