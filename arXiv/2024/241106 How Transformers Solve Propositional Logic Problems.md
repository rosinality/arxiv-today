https://arxiv.org/abs/2411.04105

*How Transformers Solve Propositional Logic Problems: A Mechanistic Analysis* (Guan Zhe Hong, Nishanth Dikkala, Enming Luo, Cyrus Rashtchian, Rina Panigrahy)

> Large language models (LLMs) have shown amazing performance on tasks that require planning and reasoning. Motivated by this, we investigate the internal mechanisms that underpin a network's ability to perform complex logical reasoning. We first construct a synthetic propositional logic problem that serves as a concrete test-bed for network training and evaluation. Crucially, this problem demands nontrivial planning to solve, but we can train a small transformer to achieve perfect accuracy. Building on our set-up, we then pursue an understanding of precisely how a three-layer transformer, trained from scratch, solves this problem. We are able to identify certain "planning" and "reasoning" circuits in the network that necessitate cooperation between the attention blocks to implement the desired logic. To expand our findings, we then study a larger model, Mistral 7B. Using activation patching, we characterize internal components that are critical in solving our logic problem. Overall, our work systemically uncovers novel aspects of small and large transformers, and continues the study of how they plan and reason.

트랜스포머가 명제 논리를 해결하기 위해 사용하는 회로 분석. Mistral 7B로 실험한 것이 꽤 재미있네요. 쿼리와 관련된 규칙을 찾는 헤드, 수집한 쿼리와 규칙 정보를 응답 위치로 옮기는 헤드, 사실을 처리하는 헤드, 그리고 최종 결정을 하는 헤드로 구성되어 있군요. 이런 구조가 형성된다는 것이 새삼 신기하긴 합니다.

<english>
Analysis on circuits in transformers which is used for solve propositional logic. Experimental results for Mistral 7B is quite interesting. There are head which finds rules related to the query, head that move informations about query and related rules, head that processes facts, and final decision making heads. It is still surprising that these kind of structured is formed in transformer.
</english>

#mechanistic-interpretation 