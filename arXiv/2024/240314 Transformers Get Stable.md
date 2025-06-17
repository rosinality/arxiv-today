https://arxiv.org/abs/2403.09635

*Transformers Get Stable: An End-to-End Signal Propagation Theory for Language Models* (Akhil Kedia, Mohd Abbas Zaidi, Sushil Khyalia, Jungho Jung, Harshith Goka, Haejun Lee)

> In spite of their huge success, transformer models remain difficult to scale in depth. In this work, we develop a unified signal propagation theory and provide formulae that govern the moments of the forward and backward signal through the transformer model. Our framework can be used to understand and mitigate vanishing/exploding gradients, rank collapse, and instability associated with high attention scores. We also propose DeepScaleLM, an initialization and scaling scheme that conserves unit output/gradient moments throughout the model, enabling the training of very deep models with 100s of layers. We find that transformer models could be much deeper - our deep models with fewer parameters outperform shallow models in Language Modeling, Speech Translation, and Image Classification, across Encoder-only, Decoder-only and Encoder-Decoder variants, for both Pre-LN and Post-LN transformers, for multiple datasets and model sizes. These improvements also translate into improved performance on downstream Question Answering tasks and improved robustness for image classification.

트랜스포머 레이어의 출력과 그래디언트의 모멘트를 유도한 다음 이를 사용해 출력과 그래디언트의 증가를 안정화하기 위한 초기화 방법을 설계했습니다. 입력에 존재하는 상관관계의 영향을 고려한 것이 재미있네요.

#transformer 