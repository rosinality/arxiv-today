https://arxiv.org/abs/2510.06673

*Heptapod: Language Modeling on Visual Signals* (Yongxin Zhu, Jiawei Chen, Yuanzhe Chen, Zhuo Chen, Dongya Jia, Jian Cong, Xiaobin Zhuang, Yuping Wang, Yuxuan Wang)

> We introduce Heptapod, an image autoregressive model that adheres to the foundational principles of language modeling. Heptapod employs \textbf{causal attention}, \textbf{eliminates reliance on CFG}, and \textbf{eschews the trend of semantic tokenizers}. Our key innovation is \textit{next 2D distribution prediction}: a causal Transformer with reconstruction-focused visual tokenizer, learns to predict the distribution over the entire 2D spatial grid of images at each timestep. This learning objective unifies the sequential modeling of autoregressive framework with the holistic self-supervised learning of masked autoencoding, enabling the model to capture comprehensive image semantics via generative training. On the ImageNet generation benchmark, Heptapod achieves an FID of $2.70$, significantly outperforming previous causal autoregressive approaches. We hope our work inspires a principled rethinking of language modeling on visual signals and beyond.

Autoregressive 이미지 생성 모델이 장거리 관계를 고려하도록 하기 위해 다음 토큰 뿐만 아니라 남은 토큰 모두를 예측하도록 강제.

<english>
Enforcing autoregressive image generation model to consider long-range dependencies by make it predict all of remaining tokens, not just a next token.
</english>

#image-generation #autoregressive-model 