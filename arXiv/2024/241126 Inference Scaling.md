https://arxiv.org/abs/2411.17501

*Inference Scaling FLaws: The Limits of LLM Resampling with Imperfect Verifiers* (Benedikt Stroebl, Sayash Kapoor, Arvind Narayanan)

> Recent research has generated hope that inference scaling could allow weaker language models to match or exceed the accuracy of stronger models, such as by repeatedly sampling solutions to a coding problem until it passes unit tests. The central thesis of this paper is that there is no free lunch for inference scaling: indefinite accuracy improvement through resampling can only be realized if the "verifier" (in this case, a set of unit tests) is perfect. When the verifier is imperfect, as it almost always is in domains such as reasoning or coding (for example, unit tests have imperfect coverage), there is a nonzero probability of false positives: incorrect solutions that pass the verifier. Resampling cannot decrease this probability, so it imposes an upper bound to the accuracy of resampling-based inference scaling even with an infinite compute budget. We find that there is a very strong correlation between the model's single-sample accuracy (i.e. accuracy without unit tests) and its false positive rate on coding benchmarks HumanEval and MBPP, whose unit tests have limited coverage. Therefore, no amount of inference scaling of weaker models can enable them to match the single-sample accuracy of a sufficiently strong model (Fig. 1a). When we consider that false positives have a negative utility compared to abstaining from producing a solution, it bends the inference scaling curve further downward. Empirically, we find that the optimal number of samples can be less than 10 under realistic assumptions (Fig. 1b). Finally, we show that beyond accuracy, false positives may have other undesirable qualities, such as poor adherence to coding style conventions.

Verifier가 불완전한 상황에서 탐색의 양을 늘리는 것은 False Positive를 늘리는 것이 될 수 있다는 주장. 문제의 난이도에 따른 패턴의 차이도 그렇고 (https://arxiv.org/abs/2408.03314) Inference Scaling Law는 Training Scaling Law에 비해 훨씬 더 복잡한 패턴이 나타날 수 있다는 생각입니다.

<english>
Argument that more search can increase false positive if verifier is incomplete. Considering pattern differences between problem difficulties (https://arxiv.org/abs/2408.03314) I think inference scaling law can cause much more complex patterns compared to training scaling law.
</english>

#search

# Links

[[240807 Search Scaling Law.md]]