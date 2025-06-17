https://arxiv.org/abs/2504.12691

*Why and How LLMs Hallucinate: Connecting the Dots with Subsequence Associations* (Yiyou Sun, Yu Gai, Lijie Chen, Abhilasha Ravichander, Yejin Choi, Dawn Song)

> Large language models (LLMs) frequently generate hallucinations-content that deviates from factual accuracy or provided context-posing challenges for diagnosis due to the complex interplay of underlying causes. This paper introduces a subsequence association framework to systematically trace and understand hallucinations. Our key insight is that hallucinations arise when dominant hallucinatory associations outweigh faithful ones. Through theoretical and empirical analyses, we demonstrate that decoder-only transformers effectively function as subsequence embedding models, with linear layers encoding input-output associations. We propose a tracing algorithm that identifies causal subsequences by analyzing hallucination probabilities across randomized input contexts. Experiments show our method outperforms standard attribution techniques in identifying hallucination causes and aligns with evidence from the model's training corpus. This work provides a unified perspective on hallucinations and a robust framework for their tracing and analysis.

할루시네이션의 원인을 입력의 서브시퀀스와 출력의 서브시퀀스 사이의 조합에서 할루시네이션에 해당하는 조합이 정확한 조합보다 연관 관계가 강하면 발생한다는 관점에서 분석했군요.

<english>
An analysis on cause of hallucations, with viewpoint of associations between subsequence in inputs and subsequence of outputs. If hallucinatory associations is stronger than faithful associations then hallucination occurs.
</english>

#hallucination #mechanistic-interpretation 