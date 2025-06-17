https://arxiv.org/abs/2501.04682

*Towards System 2 Reasoning in LLMs: Learning How to Think With Meta Chain-of-Though* (Violet Xiang, Charlie Snell, Kanishk Gandhi, Alon Albalak, Anikait Singh, Chase Blagden, Duy Phung, Rafael Rafailov, Nathan Lile, Dakota Mahan, Louis Castricato, Jan-Philipp Franken, Nick Haber, Chelsea Finn)

> We propose a novel framework, Meta Chain-of-Thought (Meta-CoT), which extends traditional Chain-of-Thought (CoT) by explicitly modeling the underlying reasoning required to arrive at a particular CoT. We present empirical evidence from state-of-the-art models exhibiting behaviors consistent with in-context search, and explore methods for producing Meta-CoT via process supervision, synthetic data generation, and search algorithms. Finally, we outline a concrete pipeline for training a model to produce Meta-CoTs, incorporating instruction tuning with linearized search traces and reinforcement learning post-training. Finally, we discuss open research questions, including scaling laws, verifier roles, and the potential for discovering novel reasoning algorithms. This work provides a theoretical and practical roadmap to enable Meta-CoT in LLMs, paving the way for more powerful and human-like reasoning in artificial intelligence.

추론 능력에 대한 방대한 탐색. 기본적인 아이디어는 CoT에 대한 CoT가 필요하다는 것입니다. CoT가 문제에 대한 해결 과정이라고 한다면 이 해결 과정을 선택하기 위한 과정이 필요하다는 것이죠. 그런데 해결 과정을 상세하게 기술한 데이터도 드물지만 그 특정한 해결 과정에 도달하기 위한 과정이 포함된 데이터는 더 찾아보기 어렵죠. 리포트에서는 이 부분을 채우기 위해서 탐색을 모델에 내재화하는 것이 필요하다는 주장을 합니다.

추론 능력에 탐색이 필요한지는 여전히 논쟁적인 주제죠. 여기서는 MCTS 기반 탐색 결과가 o1이나 R1의 추론 과정과 비슷하다는 이야기도 합니다. 다만 Gemini Flash Thinking이나 QwQ는 좀 다르다는 이야기도 하는군요. 사실 추론 능력에 도달하기 위한 방법이 하나일 필요도 없긴 합니다. (https://x.com/denny_zhou/status/1870551510741811644)

정확하게는 모델이 내부적으로 탐색을 할 수 있어야 한다는 문제에 대해서 그것을 탐색을 통해 얻은 결과를 사용해 학습시킬 것인가 혹은 스스로 탐색을 하도록 하는 어떤 레시피를 찾을 것인가의 문제라고 할 수 있겠죠.

<english>
Extensive exploration on reasoning ability. Basic idea is that we need CoT for CoT. If we consider CoT as a detailed solution step for the problem we need a process to choose a method or approach of that solution. But the data which has detailed solution steps is scarce, and the data which contains exploration steps for that specific solution method is even more scarce. So this report says that we need to internalize exploration into the model to compensate this.

It is still debating problem whether we need search for reasoning abilities. This report also says that result of search based on MCTS is similar to reasoning process of o1 or R1. But it also says that Gemini Flash Thinking or QwQ show different patterns. Actually there are no reason that there are only one way to approach reasoning capabilities. (https://x.com/denny_zhou/status/1870551510741811644)

Accurately, it is the problem of whether we employ search first and train the model with that trajectory, or we would find a recipe for train the model to search by itself, for the problem that model should have capabilities to search internally, 
</english>

#reasoning #rl #mcts #search 