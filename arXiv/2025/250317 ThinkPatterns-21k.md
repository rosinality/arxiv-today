https://arxiv.org/abs/2503.12918

*ThinkPatterns-21k: A Systematic Study on the Impact of Thinking Patterns in LLMs* (Pengcheng Wen, Jiaming Ji, Chi-Min Chan, Juntao Dai, Donghai Hong, Yaodong Yang, Sirui Han, Yike Guo)

> Large language models (LLMs) have demonstrated enhanced performance through the \textit{Thinking then Responding} paradigm, where models generate internal thoughts before final responses (aka, System 2 thinking). However, existing research lacks a systematic understanding of the mechanisms underlying how thinking patterns affect performance across model sizes. In this work, we conduct a comprehensive analysis of the impact of various thinking types on model performance and introduce ThinkPatterns-21k, a curated dataset comprising 21k instruction-response pairs (QA) collected from existing instruction-following datasets with five thinking types. For each pair, we augment it with five distinct internal thinking patterns: one unstructured thinking (monologue) and four structured variants (decomposition, self-ask, self-debate and self-critic), while maintaining the same instruction and response. Through extensive evaluation across different model sizes (3B-32B parameters), we have two key findings: (1) smaller models (<30B parameters) can benefit from most of structured thinking patterns, while larger models (32B) with structured thinking like decomposition would degrade performance and (2) unstructured monologue demonstrates broad effectiveness across different model sizes. Finally, we released all of our datasets, checkpoints, training logs of diverse thinking patterns to reproducibility, aiming to facilitate further research in this direction.

다섯 가지의 사고 패턴을 디자인한 다음 그 패턴을 따르는 응답들을 생성해서 학습 결과를 평가해봤군요. 채팅 벤치 기준이고 각 패턴에 대해 생성할 수 있는 응답의 평균 퀄리티 등도 문제가 되겠습니다만, 특정한 구조가 없는 사고 패턴이 가장 유리하다는 것은 자연스럽네요.

<english>
The authors designed 5 thought patterns and generated responses following it, and evaluated training results. It is based on chat benches and average quality of responses that can be generated for each patterns would be problem, but it is natural to thought patterns without specific structures is most advantageous.
</english>

#reasoning 