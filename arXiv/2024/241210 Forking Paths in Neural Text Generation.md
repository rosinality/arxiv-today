https://arxiv.org/abs/2412.07961

*Forking Paths in Neural Text Generation* (Eric Bigelow, Ari Holtzman, Hidenori Tanaka, Tomer Ullman)

> Estimating uncertainty in Large Language Models (LLMs) is important for properly evaluating LLMs, and ensuring safety for users. However, prior approaches to uncertainty estimation focus on the final answer in generated text, ignoring intermediate steps that might dramatically impact the outcome. We hypothesize that there exist key forking tokens, such that re-sampling the system at those specific tokens, but not others, leads to very different outcomes. To test this empirically, we develop a novel approach to representing uncertainty dynamics across individual tokens of text generation, and applying statistical models to test our hypothesis. Our approach is highly flexible: it can be applied to any dataset and any LLM, without fine tuning or accessing model weights. We use our method to analyze LLM responses on 7 different tasks across 4 domains, spanning a wide range of typical use cases. We find many examples of forking tokens, including surprising ones such as punctuation marks, suggesting that LLMs are often just a single token away from saying something very different.

텍스트 생성 과정에서 다른 토큰으로 대체된다면 생성 결과를 크게 바꿀 수 있는 토큰이 있다는 가설. 각 토큰에 대해 다른 토큰을 샘플링해서 텍스틀 생성한 다음 생성 결과의 차이를 측정합니다. 그리고 시퀀스 내에서 이 차이를 크게 유발하는 지점이 있는지를 Change Point Detection과 생존 분석으로 분석했네요. 얼마 전에도 추론에 결정적인 토큰이 존재한다는 연구가 있었죠. (https://arxiv.org/abs/2411.19943) 재미있는 지점이네요.

<english>
A hypothesis that there are token that if it is replaced by another tokens then it will result in very different outcomes during text generation. This study measures difference in generation outcomes by sampling another tokens for each tokens in sequences and generating rest of the tokens. And they analyzed whether there is a point that causes large outcome differences in the sequence using change point detection and survival analysis. Recently there was a research insist that there is critical token that affects reasoning outcomes. (https://arxiv.org/abs/2411.19943) I think it is an interesting point.
</english>

#llm

# Links

[[241129 Critical Tokens Matter.md]]