https://arxiv.org/abs/2410.01748

*Not All LLM Reasoners Are Created Equal* (Arian Hosseini, Alessandro Sordoni, Daniel Toyama, Aaron Courville, Rishabh Agarwal)

> We study the depth of grade-school math (GSM) problem-solving capabilities of LLMs. To this end, we evaluate their performance on pairs of existing math word problems together so that the answer to the second problem depends on correctly answering the first problem. Our findings reveal a significant reasoning gap in most LLMs, that is performance difference between solving the compositional pairs and solving each question independently. This gap is more pronounced in smaller, more cost-efficient, and math-specialized models. Moreover, instruction-tuning recipes and code generation have varying effects across LLM sizes, while finetuning on GSM can lead to task overfitting. Our analysis indicates that large reasoning gaps are not because of test-set leakage, but due to distraction from additional context and poor second-hop reasoning. Overall, LLMs exhibit systematic differences in their reasoning abilities, despite what their performance on standard benchmarks indicates.

GSM8K 문제들을 이어붙여서 복합 문제를 만든 다음 평가. 문제를 연결해서 추론 난이도를 높이는 연구는 최근에도 나왔었죠. (https://arxiv.org/abs/2410.00151)

흥미로운 지점은 모델 크기와 Instruction Tuning의 전후 성능 차이를 분석한 부분이네요. 작은 모델에서는 Instruction Tuning으로 성능을 크게 올릴 수 있지만 그것이 실용적인 성능 차이로는 이어지지 않을 수 있다는 것이죠.

<english>
Evaluate LLMs on composition problems made by concatenating GSM8K problems. Recently there was also approach that combining problems to increase difficulties of reasoning. (https://arxiv.org/abs/2410.00151)

Interesting point is on analysis of comparing difference of perfomrnaces of before or after instruction tuning, respect to model sizes. In small models you can increase performance on benchmark greatly with instruction tuning, but it maybe not related to actual, practical performances.
</english>

#benchmark #llm #reasoning

# Links

