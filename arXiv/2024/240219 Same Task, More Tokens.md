https://arxiv.org/abs/2402.14848

*Same Task, More Tokens: the Impact of Input Length on the Reasoning Performance of Large Language Models* (Mosh Levy, Alon Jacoby, Yoav Goldberg)

> This paper explores the impact of extending input lengths on the capabilities of Large Language Models (LLMs). Despite LLMs advancements in recent times, their performance consistency across different input lengths is not well understood. We investigate this aspect by introducing a novel QA reasoning framework, specifically designed to assess the impact of input length. We isolate the effect of input length using multiple versions of the same sample, each being extended with padding of different lengths, types and locations. Our findings show a notable degradation in LLMs' reasoning performance at much shorter input lengths than their technical maximum. We show that the degradation trend appears in every version of our dataset, although at different intensities. Additionally, our study reveals that traditional perplexity metrics do not correlate with performance of LLMs' in long input reasoning tasks. We analyse our results and identify failure modes that can serve as useful guides for future research, potentially informing strategies to address the limitations observed in LLMs.

Long Context 벤치마크. 질문에 응답하는데 필요한 문단을 두 개 설정해서 이 문단들을 전체 Context에 서로 다른 위치에 배치한 다음 평가하는 방법. 문단 두 개 사이에는 이 두 문단을 복사하거나 관계 없는 텍스트로 채우는 방법 등을 사용합니다.

Context Length 증가에 따라 토큰 예측 성능은 올라가지만 QA 성능은 유의미하게 낮아지는 패턴이 나타나네요. 이유가 뭘까요? 여전히 Instruction Tuning 과정의 문제가 아닐까 하는 추측은 하게 됩니다.

#long-context #benchmark 