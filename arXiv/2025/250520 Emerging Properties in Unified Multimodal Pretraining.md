https://arxiv.org/abs/2505.14683

*Emerging Properties in Unified Multimodal Pretraining* (Chaorui Deng, Deyao Zhu, Kunchang Li, Chenhui Gou, Feng Li, Zeyu Wang, Shu Zhong, Weihao Yu, Xiaonan Nie, Ziang Song, Guang Shi, Haoqi Fan)

> Unifying multimodal understanding and generation has shown impressive capabilities in cutting-edge proprietary systems. In this work, we introduce BAGEL, an open0source foundational model that natively supports multimodal understanding and generation. BAGEL is a unified, decoder0only model pretrained on trillions of tokens curated from large0scale interleaved text, image, video, and web data. When scaled with such diverse multimodal interleaved data, BAGEL exhibits emerging capabilities in complex multimodal reasoning. As a result, it significantly outperforms open-source unified models in both multimodal generation and understanding across standard benchmarks, while exhibiting advanced multimodal reasoning abilities such as free-form image manipulation, future frame prediction, 3D manipulation, and world navigation. In the hope of facilitating further opportunities for multimodal research, we share the key findings, pretraining details, data creation protocal, and release our code and checkpoints to the community. The project page is at https://bagel-ai.org/

바이트댄스의 이미지 인식/생성 모델. 요즘 많이 시도하는 것처럼 ViT와 VAE 토큰을 동시 사용하고 Diffusion을 사용, 그리고 트랜스포머 백본을 중복시키는 MoT를 사용했군요 (https://arxiv.org/abs/2411.04996).

학습 데이터 증가에 따라 특히 생성 영역에서 창발이 나타나네요.

<english>
ByteDance's image understanding-generation model. They use ViT and VAE tokens simultaneously, as commonly tried recently, and used diffusion and MoT that duplicates transformer backbone (https://arxiv.org/abs/2411.04996).

Emergent phenomena occurs along with training data increases, especially on generation tasks.
</english>

#multimodal #image-generation 