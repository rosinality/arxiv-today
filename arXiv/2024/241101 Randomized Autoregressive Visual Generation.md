https://arxiv.org/abs/2411.00776

*Randomized Autoregressive Visual Generation* (Qihang Yu, Ju He, Xueqing Deng, Xiaohui Shen, Liang-Chieh Chen)

> This paper presents Randomized AutoRegressive modeling (RAR) for visual generation, which sets a new state-of-the-art performance on the image generation task while maintaining full compatibility with language modeling frameworks. The proposed RAR is simple: during a standard autoregressive training process with a next-token prediction objective, the input sequence-typically ordered in raster form-is randomly permuted into different factorization orders with a probability r, where r starts at 1 and linearly decays to 0 over the course of training. This annealing training strategy enables the model to learn to maximize the expected likelihood over all factorization orders and thus effectively improve the model's capability of modeling bidirectional contexts. Importantly, RAR preserves the integrity of the autoregressive modeling framework, ensuring full compatibility with language modeling while significantly improving performance in image generation. On the ImageNet-256 benchmark, RAR achieves an FID score of 1.48, not only surpassing prior state-of-the-art autoregressive image generators but also outperforming leading diffusion-based and masked transformer-based methods. Code and models will be made available at https://github.com/bytedance/1d-tokenizer

Autoregressive 이미지 생성에서 이미지 시퀀스의 Permutation을 통해 학습시키면 성능이 향상된다는 연구. 학습 과정에서 Permutation한 이미지에 노출됐다는 것이 생성에 어떤 영향을 미치는지 연결하기가 쉽지는 않네요. (다양한 배치와 패턴의 패치를 통해 좀 더 강인한 거동을 학습할 수 있다는 생각은 듭니다.)

<english>
A study that performance of the autoregressive image generation model can be enhanced by train it on permutation of image sequences. It is hard to connect that models is exposed on permuted images to the effect on generation processes. (I think is is possible to model have more robust behavior by trained on various arrangements and patterns of image patches.)
</english>

#image-generation #autoregressive-model 