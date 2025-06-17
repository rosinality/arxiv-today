https://arxiv.org/abs/2502.01612

*Self-Improving Transformers Overcome Easy-to-Hard and Length Generalization Challenges* (Nayoung Lee, Ziyang Cai, Avi Schwarzschild, Kangwook Lee, Dimitris Papailiopoulos)

> Large language models often struggle with length generalization and solving complex problem instances beyond their training distribution. We present a self-improvement approach where models iteratively generate and learn from their own solutions, progressively tackling harder problems while maintaining a standard transformer architecture. Across diverse tasks including arithmetic, string manipulation, and maze solving, self-improving enables models to solve problems far beyond their initial training distribution-for instance, generalizing from 10-digit to 100-digit addition without apparent saturation. We observe that in some cases filtering for correct self-generated examples leads to exponential improvements in out-of-distribution performance across training rounds. Additionally, starting from pretrained models significantly accelerates this self-improvement process for several tasks. Our results demonstrate how controlled weak-to-strong curricula can systematically teach a model logical extrapolation without any changes to the positional embeddings, or the model architecture.

연산 문제 등에 대해서 길이 일반화를 시도한 방법. 짧은 길이에 대해 학습시킨 다음 긴 길이에 대한 모델 생성 결과를 길이와 Majority Voting으로 필터링해서 학습시켰습니다. 이전에 Chain of Thought로 길이를 점진적으로 증가시켰던 연구가(https://arxiv.org/abs/2309.08589) 생각나네요.

<english>
The study tried length generalization for problems like arithmetic. They trained a model using the data generated from it and filtered using length and majority voting, after train it on short length. It reminds me a study tried to extrapolate length progressively using chain of thought (https://arxiv.org/abs/2309.08589).
</english>

#extrapolation #synthetic-data #self-improvement

# Links

[[230915 Chain-of-Thought Reasoning is a Policy Improvement Operator.md]]