https://arxiv.org/abs/2410.01792

*When a language model is optimized for reasoning, does it still show embers of autoregression? An analysis of OpenAI o1* (R. Thomas McCoy, Shunyu Yao, Dan Friedman, Mathew D. Hardy, Thomas L. Griffiths)

> In "Embers of Autoregression" (McCoy et al., 2023), we showed that several large language models (LLMs) have some important limitations that are attributable to their origins in next-word prediction. Here we investigate whether these issues persist with o1, a new system from OpenAI that differs from previous LLMs in that it is optimized for reasoning. We find that o1 substantially outperforms previous LLMs in many cases, with particularly large improvements on rare variants of common tasks (e.g., forming acronyms from the second letter of each word in a list, rather than the first letter). Despite these quantitative improvements, however, o1 still displays the same qualitative trends that we observed in previous systems. Specifically, o1 - like previous LLMs - is sensitive to the probability of examples and tasks, performing better and requiring fewer "thinking tokens" in high-probability settings than in low-probability ones. These results show that optimizing a language model for reasoning can mitigate but might not fully overcome the language model's probability sensitivity.

Embers of Autoregression을 (https://arxiv.org/abs/2309.13638) o1에 대해 테스트해봤군요. 여전히 Autoregressive 학습에 의한 과제 빈도에 따른 성능 변화가 나타나지만 그 정도가 훨씬 나아지긴 했습니다.

한 가지 재미있는 것은 빈도가 낮은 과제일수록 생성하는 Reasoning 토큰의 수도 늘어난다는 것이네요.

o1은 굉장히 중요한 발전이고 과거의 LLM과는 질적으로 다른 모델이 될 수 있다는 생각이 강해집니다. 너무 당연한 이야기일까요?

<english>
Evaluation of o1 on problems from Embers of Autoregression. (https://arxiv.org/abs/2309.13638) Although there are still performance difference by the task frequences, it is greatly alleviated.

One interesting point is that number of generated reasoning tokens are increased if task frequencies is lower.

It seems like that o1 is very important advances and maybe it could be qualitatively different model from previous LLMs. Is it too obvious to say?
</english>

#autoregressive-model

# Links

[[230924 Embers of Autoregression.md]]