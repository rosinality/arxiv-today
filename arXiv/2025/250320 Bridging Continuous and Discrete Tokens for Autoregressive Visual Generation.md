https://arxiv.org/abs/2503.16430

*Bridging Continuous and Discrete Tokens for Autoregressive Visual Generation* (Yuqing Wang, Zhijie Lin, Yao Teng, Yuanzhi Zhu, Shuhuai Ren, Jiashi Feng, Xihui Liu)

> Autoregressive visual generation models typically rely on tokenizers to compress images into tokens that can be predicted sequentially. A fundamental dilemma exists in token representation: discrete tokens enable straightforward modeling with standard cross-entropy loss, but suffer from information loss and tokenizer training instability; continuous tokens better preserve visual details, but require complex distribution modeling, complicating the generation pipeline. In this paper, we propose TokenBridge, which bridges this gap by maintaining the strong representation capacity of continuous tokens while preserving the modeling simplicity of discrete tokens. To achieve this, we decouple discretization from the tokenizer training process through post-training quantization that directly obtains discrete tokens from continuous representations. Specifically, we introduce a dimension-wise quantization strategy that independently discretizes each feature dimension, paired with a lightweight autoregressive prediction mechanism that efficiently model the resulting large token space. Extensive experiments show that our approach achieves reconstruction and generation quality on par with continuous methods while using standard categorical prediction. This work demonstrates that bridging discrete and continuous paradigms can effectively harness the strengths of both approaches, providing a promising direction for high-quality visual generation with simple autoregressive modeling. Project page: https://yuqingwang1029.github.io/TokenBridge.

VQ를 학습하는 대신 VAE를 학습하고 Feature를 Quantization해서 Discrete Token을 만드는 방법. 각 채널마다 각각 토큰이 할당되기 때문에 각 채널에 대해 Autoregressive 생성을 했습니다.

여담이지만 각 채널을 64개의 Vocabulary로 분할했는데 이건 실질적으로 VAE Feature가 각 채널 당 4bit 정도의 정보를 갖는다는 의미겠네요.

<english>
Instead of training VQ, train VAE and extracts discrete tokens by quantizing features. As tokens are assigned to each channels autoregressive generation was done for each channels.

By the way, they splitted each channels into 64 vocabularies, and it would mean that essentially VAE feature has about 4 bit informations per channels.
</english>

#vq #quantization #tokenizer 