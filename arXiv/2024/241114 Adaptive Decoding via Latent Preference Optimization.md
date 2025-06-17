https://arxiv.org/abs/2411.09661

*Adaptive Decoding via Latent Preference Optimization* (Shehzaad Dhuliawala, Ilia Kulikov, Ping Yu, Asli Celikyilmaz, Jason Weston, Sainbayar Sukhbaatar, Jack Lanchantin)

> During language model decoding, it is known that using higher temperature sampling gives more creative responses, while lower temperatures are more factually accurate. However, such models are commonly applied to general instruction following, which involves both creative and fact seeking tasks, using a single fixed temperature across all examples and tokens. In this work, we introduce Adaptive Decoding, a layer added to the model to select the sampling temperature dynamically at inference time, at either the token or example level, in order to optimize performance. To learn its parameters we introduce Latent Preference Optimization (LPO) a general approach to train discrete latent variables such as choices of temperature. Our method outperforms all fixed decoding temperatures across a range of tasks that require different temperatures, including UltraFeedback, Creative Story Writing, and GSM8K.

샘플 단위 혹은 토큰 단위로 적절한 Temperature를 설정하는 모델 학습시키기. 토큰 단위 Temperature는 꽤 흥미로운 방향일 듯 하네요. 창조적이어야 할 부분에 대해서만 Temperature를 높인다거나 하는 가능성이 나타날 수 있겠죠.

<english>
Training a model sets appropriate temperature per each samples or tokens. I think setting temperature for each token differently is quite intersting direction to explore. It allows the possibility of increasing temperature for portions that should be creative.
</english>

#alignment #rlhf 