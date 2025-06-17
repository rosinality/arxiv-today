https://arxiv.org/abs/2402.08147

*Verified Multi-Step Synthesis using Large Language Models and Monte Carlo Tree Search* (David Brandfonbrener, Sibi Raja, Tarun Prasad, Chloe Loughridge, Jianang Yang, Simon Henniger, William E. Byrd, Robert Zinkov, Nada Amin)

> We present an approach using Monte Carlo Tree Search (MCTS) to guide Large Language Models (LLMs) to generate verified programs in Dafny, Lean and Coq. Our method, which we call VMCTS, leverages the verifier inside the search algorithm by checking partial programs at each step. In combination with the LLM prior, the verifier feedback raises the synthesis capabilities of open source models. On a set of five verified programming problems, we find that in four problems where the base model cannot solve the question even when re-sampling solutions for one hour, VMCTS can solve the problems within 6 minutes. The base model with VMCTS is even competitive with ChatGPT4 augmented with plugins and multiple re-tries on these problems. Our code and benchmarks are available at https://github.com/namin/llm-verified-with-monte-carlo-tree-search .

LLM 디코딩 과정에서 트리 서치를 하면서 Dafny/Coq/Lean 같은 검증 능력이 있는 프로그래밍 언어를 사용해 검증해나가는 시도. Lean 같은 언어로 무언가를 할 수 있지 않을까 하는 생각들이 나왔었는데 그 사례가 될 것 같네요.

#decoding #search 