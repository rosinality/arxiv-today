https://arxiv.org/abs/2504.01935

*Critical Thinking: Which Kinds of Complexity Govern Optimal Reasoning Length?* (Celine Lee, Alexander M. Rush, Keyon Vafa)

> Large language models (LLMs) often benefit from verbalized reasoning at inference time, but it remains unclear which aspects of task difficulty these extra reasoning tokens address. To investigate this question, we formalize a framework using deterministic finite automata (DFAs). DFAs offer a formalism through which we can characterize task complexity through measurable properties such as run length (number of reasoning steps required) and state-space size (decision complexity). We first show that across different tasks and models of different sizes and training paradigms, there exists an optimal amount of reasoning tokens such that the probability of producing a correct solution is maximized. We then investigate which properties of complexity govern this critical length: we find that task instances with longer corresponding underlying DFA runs (i.e. demand greater latent state-tracking requirements) correlate with longer reasoning lengths, but, surprisingly, that DFA size (i.e. state-space complexity) does not. We then demonstrate an implication of these findings: being able to predict the optimal number of reasoning tokens for new problems and filtering out non-optimal length answers results in consistent accuracy improvements.

DFA로 표현할 수 있는 과제에서 최적 추론 길이가 어떻게 변화하는지에 대한 분석. DFA의 상태의 수에는 큰 상관이 없고 실행 시간에 영향을 받는다고 하는군요.

<english>
Analysis on change of optimal reasoning length on tasks that can be represented in DFA. The study says it is largely irrelevant on number of states, and affected mainly from run length.
</english>

#reasoning 