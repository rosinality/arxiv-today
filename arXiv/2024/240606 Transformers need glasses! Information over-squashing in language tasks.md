https://arxiv.org/abs/2406.04267

*Transformers need glasses! Information over-squashing in language tasks* (Federico Barbero, Andrea Banino, Steven Kapturowski, Dharshan Kumaran, João G.M. Araújo, Alex Vitvitskyi, Razvan Pascanu, Petar Veličković)

> We study how information propagates in decoder-only Transformers, which are the architectural backbone of most existing frontier large language models (LLMs). We rely on a theoretical signal propagation analysis -- specifically, we analyse the representations of the last token in the final layer of the Transformer, as this is the representation used for next-token prediction. Our analysis reveals a representational collapse phenomenon: we prove that certain distinct sequences of inputs to the Transformer can yield arbitrarily close representations in the final token. This effect is exacerbated by the low-precision floating-point formats frequently used in modern LLMs. As a result, the model is provably unable to respond to these sequences in different ways -- leading to errors in, e.g., tasks involving counting or copying. Further, we show that decoder-only Transformer language models can lose sensitivity to specific tokens in the input, which relates to the well-known phenomenon of over-squashing in graph neural networks. We provide empirical evidence supporting our claims on contemporary LLMs. Our theory also points to simple solutions towards ameliorating these issues.

트랜스포머에서 서로 다른 입력에 대해 임베딩 Representation이 같아지는 문제(Representational Collapse), 토큰의 변화에 따른 출력의 변화가 토큰의 위치에 따라 달라지는 문제를 다루고 있습니다.

Self Attention이 Low Pass Filter (https://arxiv.org/abs/2202.06709) 라는 아이디어가 생각나네요. 연결 지점이 있지 않을까 싶습니다.

#transformer

# Links

[[220214 How Do Vision Transformers Work.md]]