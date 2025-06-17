https://arxiv.org/abs/2310.02304

Self-Taught Optimizer (STOP): Recursively Self-Improving Code Generation (Eric Zelikman, Eliana Lorch, Lester Mackey, Adam Tauman Kalai)

LLM을 사용해서 과제의 답변을 개선하는 프로그램인 Improver를 가정해보죠. 간단하게 이 답변을 개선해보라고 하는 프롬프트를 사용하는 프로그램을 생각해볼 수 있겠죠. 이 논문은 이 Improver를 Improver를 사용해 개선할 수 있는가라는 문제를 다룹니다. 실제로 개선이 되고 개선된 Improver가 다른 과제에도 일반화가 가능하군요.

이렇게 찾아낸 Improver들을 보니 Beam Search나 Simulated Annealing, Bandit 등을 사용하는 알고리즘이 나타났다고 하네요. 이건 예를 들어 Tree of Thoughts (https://arxiv.org/abs/2305.10601) 같은 알고리즘을 LLM을 사용해 찾아낼 수 있다는 것을 시사한다고 할 수 있겠죠. 좀 충격적이네요.

#refinement

# Links

[[230517 Tree of Thoughts.md]]