https://arxiv.org/abs/2402.09371

*Transformers Can Achieve Length Generalization But Not Robustly* (Yongchao Zhou, Uri Alon, Xinyun Chen, Xuezhi Wang, Rishabh Agarwal, Denny Zhou)

> Length generalization, defined as the ability to extrapolate from shorter training sequences to longer test ones, is a significant challenge for language models. This issue persists even with large-scale Transformers handling relatively straightforward tasks. In this paper, we test the Transformer's ability of length generalization using the task of addition of two integers. We show that the success of length generalization is intricately linked to the data format and the type of position encoding. Using the right combination of data format and position encodings, we show for the first time that standard Transformers can extrapolate to a sequence length that is 2.5x the input length. Nevertheless, unlike in-distribution generalization, length generalization remains fragile, significantly influenced by factors like random weight initialization and training data order, leading to large variances across different random seeds.

트랜스포머의 Length Generalization 연구. 덧셈에 대해서 테스트했는데 FIRE (https://arxiv.org/abs/2310.04418), 숫자 순서 뒤집기, 자릿수에 대한 힌트, 거기에 추가적으로 Randomized PE (https://arxiv.org/abs/2305.16843) 까지 더했습니다. 사실 Randomized PE를 쓰면 테스트 분포의 PE까지 들어오기 때문에 좀 반칙이 아닌가 싶긴 하네요.

그렇지만 이 모든 트릭을 결합해도 Weight의 초기화 시드나 학습 데이터의 순서에 따라 성능이 크게 달라지는군요. Length Generalization은 운이 좋으면 나타나는 특성으로 보입니다.

Positional Encoding은 대칭성에 관한 문제일 것이고 숫자의 순서를 뒤집는다거나 하는 것은 Causal LM의 특성과 관련된 문제겠죠. 아직 이에 대한 확실한 해법이 없네요.

#transformer #long-context

# Links

[[231006 Functional Interpolation for Relative Positions Improves Long Context Transformers.md]]