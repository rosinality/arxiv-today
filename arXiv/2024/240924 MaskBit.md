https://arxiv.org/abs/2409.16211

*MaskBit: Embedding-free Image Generation via Bit Tokens* (Mark Weber, Lijun Yu, Qihang Yu, Xueqing Deng, Xiaohui Shen, Daniel Cremers, Liang-Chieh Chen)

> Masked transformer models for class-conditional image generation have become a compelling alternative to diffusion models. Typically comprising two stages - an initial VQGAN model for transitioning between latent space and image space, and a subsequent Transformer model for image generation within latent space - these frameworks offer promising avenues for image synthesis. In this study, we present two primary contributions: Firstly, an empirical and systematic examination of VQGANs, leading to a modernized VQGAN. Secondly, a novel embedding-free generation network operating directly on bit tokens - a binary quantized representation of tokens with rich semantics. The first contribution furnishes a transparent, reproducible, and high-performing VQGAN model, enhancing accessibility and matching the performance of current state-of-the-art methods while revealing previously undisclosed details. The second contribution demonstrates that embedding-free image generation using bit tokens achieves a new state-of-the-art FID of 1.52 on the ImageNet 256x256 benchmark, with a compact generator model of mere 305M parameters.

VQGAN을 개선하면서 Lookup-Free Quantization을 적용. (https://arxiv.org/abs/2310.05737) LFQ를 적용하면 K 차원의 바이너리 코드가 나오니 굳이 임베딩을 사용해서 변환하지 않고 그대로 Feature로 사용. 이 코드에 구조가 있다는 것을 발견했고 (즉 코드가 유사하면 결과도 유사) Masked Image Generation으로 이미지를 생성할 때에도 임베딩 없이 입력으로 사용하는군요. (출력은 여전히 2^K개 클래스 분류인 것 같긴 하네요.)

#vq #image-generation #mlm

# Links

[[231009 Language Model Beats Diffusion -- Tokenizer is Key to Visual Generation.md]]