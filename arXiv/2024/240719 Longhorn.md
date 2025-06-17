https://arxiv.org/abs/2407.14207

*Longhorn: State Space Models are Amortized Online Learners* (Bo Liu, Rui Wang, Lemeng Wu, Yihao Feng, Peter Stone, Qiang Liu)

> The most fundamental capability of modern AI methods such as Large Language Models (LLMs) is the ability to predict the next token in a long sequence of tokens, known as ``sequence modeling." Although the Transformers model is the current dominant approach to sequence modeling, its quadratic computational cost with respect to sequence length is a significant drawback. State-space models (SSMs) offer a promising alternative due to their linear decoding efficiency and high parallelizability during training. However, existing SSMs often rely on seemingly ad hoc linear recurrence designs. In this work, we explore SSM design through the lens of online learning, conceptualizing SSMs as meta-modules for specific online learning problems. This approach links SSM design to formulating precise online learning objectives, with state transition rules derived from optimizing these objectives. Based on this insight, we introduce a novel deep SSM architecture based on the implicit update for optimizing an online regression objective. Our experimental results show that our models outperform state-of-the-art SSMs, including the Mamba model, on standard sequence modeling benchmarks and language modeling tasks.

State를 어떤 Objective에 학습하는 과정으로 State Space Model을 해석해서 SSM을 디자인한 사례. 얼마 전에도 비슷한 아이디어가 나왔었죠. (https://arxiv.org/abs/2406.06484, https://arxiv.org/abs/2407.04620) 꽤 흥미로운 방향인 것 같습니다.

#state-space-model

# Links

