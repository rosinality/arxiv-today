https://arxiv.org/abs/2406.02543

*To Believe or Not to Believe Your LLM* (Yasin Abbasi Yadkori, Ilja Kuzborskij, András György, Csaba Szepesvári)

> We explore uncertainty quantification in large language models (LLMs), with the goal to identify when uncertainty in responses given a query is large. We simultaneously consider both epistemic and aleatoric uncertainties, where the former comes from the lack of knowledge about the ground truth (such as about facts or the language), and the latter comes from irreducible randomness (such as multiple possible answers). In particular, we derive an information-theoretic metric that allows to reliably detect when only epistemic uncertainty is large, in which case the output of the model is unreliable. This condition can be computed based solely on the output of the model obtained simply by some special iterative prompting based on the previous responses. Such quantification, for instance, allows to detect hallucinations (cases when epistemic uncertainty is high) in both single- and multi-answer responses. This is in contrast to many standard uncertainty quantification strategies (such as thresholding the log-likelihood of a response) where hallucinations in the multi-answer case cannot be detected. We conduct a series of experiments which demonstrate the advantage of our formulation. Further, our investigations shed some light on how the probabilities assigned to a given output by an LLM can be amplified by iterative prompting, which might be of independent interest.

Epistemic Uncertainty의 측면에서 할루시네이션에 접근. 간단하게 요약하면 질문을 주고 답변을 생성합니다. 이 생성한 답변을 프롬프트에 더해서 다시 답변을 생성합니다. 이렇게 쭉 답변을 생성했을 때 답변이 이전 답변에 의존하지 않는다면 Ground Truth이고 답변이 이전 답변에 영향을 크게 받는다면 할루시네이션일 가능성이 높다는 것입니다.

실제 할루시네이션 검증은 위의 방법으로 생성한 답변 분포의 Mutual Information을 측정하는 방식으로 접근했습니다.

#hallucination 