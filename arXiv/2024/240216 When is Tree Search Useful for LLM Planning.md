https://arxiv.org/abs/2402.10890

*When is Tree Search Useful for LLM Planning? It Depends on the Discriminator* (Ziru Chen, Michael White, Raymond Mooney, Ali Payani, Yu Su, Huan Sun)

> In this paper, we examine how large language models (LLMs) solve multi-step problems under a language agent framework with three components: a generator, a discriminator, and a planning method. We investigate the practical utility of two advanced planning methods, iterative correction and tree search. We present a comprehensive analysis of how discrimination accuracy affects the overall performance of agents when using these two methods or a simpler method, re-ranking. Experiments on two tasks, text-to-SQL parsing and mathematical reasoning, show that: (1) advanced planning methods demand discriminators with at least 90% accuracy to achieve significant improvements over re-ranking; (2) current LLMs' discrimination abilities have not met the needs of advanced planning methods to achieve such improvements; (3) with LLM-based discriminators, advanced planning methods may not adequately balance accuracy and efficiency. For example, compared to the other two methods, tree search is at least 10--20 times slower but leads to negligible performance gains, which hinders its real-world applications. Code and data will be released at https://github.com/OSU-NLP-Group/llm-planning-eval.

LLM의 응답을 서치할 때 응답을 평가하는 Discriminator의 성능이 결과에 미치는 영향. Text2SQL과 GSM8K에 대해 테스트했는데 Greedy하게 샘플링하는 것보다 나은 성능을 보이려면 Discriminator의 성능이 80 - 90% 이상이 되어야 하고, 트리 서치 같은 보다 복잡한 방법은 성능 요구치가 더 높다는 발견입니다.

서치 알고리즘 자체보다도 탐색의 기준이 되는 피드백을 어떻게 설정할 것인가가 당연하게도 더 어려운 문제겠죠. 정확한 피드백을 얻기 쉬운 문제로 국한하자면 범위가 좁고요.

#search 