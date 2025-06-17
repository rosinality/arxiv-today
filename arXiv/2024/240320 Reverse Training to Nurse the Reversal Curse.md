https://arxiv.org/abs/2403.13799

*Reverse Training to Nurse the Reversal Curse* (Olga Golovneva, Zeyuan Allen-Zhu, Jason Weston, Sainbayar Sukhbaatar)

> Large language models (LLMs) have a surprising failure: when trained on "A has a feature B", they do not generalize to "B is a feature of A", which is termed the Reversal Curse. Even when training with trillions of tokens this issue still appears due to Zipf's law - hence even if we train on the entire internet. This work proposes an alternative training scheme, called reverse training, whereby all words are used twice, doubling the amount of available tokens. The LLM is trained in both forward and reverse directions by reversing the training strings while preserving (i.e., not reversing) chosen substrings, such as entities. We show that data-matched reverse-trained models provide superior performance to standard models on standard tasks, and compute-matched reverse-trained models provide far superior performance on reversal tasks, helping resolve the reversal curse issue.

Reversal Curse (https://arxiv.org/abs/2309.12288) 가 화제가 되니 Reversal Curse를 타겟해서 해소하려는 시도들도 나오더군요. (https://arxiv.org/abs/2403.00758) 시퀀스를 뒤집어서 학습시키는 것이 대안입니다.

아키텍처와 학습 Objective에 대한 좀 더 깊은 시사점이 있는 문제라고 생각해서 이 문제 자체를 핀포인트로 타겟하는 것이 그렇게 내키지는 않긴 합니다. Augmentation으로 쓸 수 있지 않을까 하는 생각이 들었고 논문에서도 그걸 암시하긴 합니다만 증거가 충분하진 않네요.

#llm

# Links

[[230921 The Reversal Curse.md]]