https://arxiv.org/abs/2402.10200

*Chain-of-Thought Reasoning Without Prompting* (Xuezhi Wang, Denny Zhou)

> In enhancing the reasoning capabilities of large language models (LLMs), prior research primarily focuses on specific prompting techniques such as few-shot or zero-shot chain-of-thought (CoT) prompting. These methods, while effective, often involve manually intensive prompt engineering. Our study takes a novel approach by asking: Can LLMs reason effectively without prompting? Our findings reveal that, intriguingly, CoT reasoning paths can be elicited from pre-trained LLMs by simply altering the \textit{decoding} process. Rather than conventional greedy decoding, we investigate the top-$k$ alternative tokens, uncovering that CoT paths are frequently inherent in these sequences. This approach not only bypasses the confounders of prompting but also allows us to assess the LLMs' \textit{intrinsic} reasoning abilities. Moreover, we observe that the presence of a CoT in the decoding path correlates with a higher confidence in the model's decoded answer. This confidence metric effectively differentiates between CoT and non-CoT paths. Extensive empirical studies on various reasoning benchmarks show that the proposed CoT-decoding substantially outperforms the standard greedy decoding.

Chain of Thought 프롬프팅 없이 Chain of Thought를 유도하기. LLM에서 응답할 때 Greedy 디코딩을 하는 것이 아니라 Top-K 토큰 중 특정 토큰으로 시작하게 하면 (그리고 나머지 토큰은 그냥 Greedy 디코딩을 하더라도) Chain of Thought 같은 추론이 발생한다는 결과입니다.

그래서 어떤 토큰으로 시작해야 하는가? 이렇게 디코딩을 하면 정답으로 이어지는 경우에는 Confidence가 더 높다고 합니다.

바로 답을 하려고 하는 경향이 LLM의 문제라고 하는데 그걸 살짝 억제해주면 좋은 패턴이 나타날 수 있다는 사례네요.

#prompt #decoding