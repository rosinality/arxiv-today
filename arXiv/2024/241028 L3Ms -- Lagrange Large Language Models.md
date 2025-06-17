https://arxiv.org/abs/2410.21533

*L3Ms -- Lagrange Large Language Models* (Guneet S. Dhillon, Xingjian Shi, Yee Whye Teh, Alex Smola)

> Supervised fine-tuning (SFT) and alignment of large language models (LLMs) are key steps in providing a good user experience. However, the concept of an appropriate alignment is inherently application-dependent, and current methods often rely on heuristic choices to drive the optimization. In this work, we formulate SFT and alignment as a constrained optimization problem, where the LLM is trained on a task while being required to meet application-specific requirements, without resorting to heuristics. To solve this, we propose Lagrange Large Language Models (L3Ms), which employ logarithmic barriers to enforce the constraints. This approach allows for the customization of L3Ms across diverse applications while avoiding heuristic-driven processes. We demonstrate experimentally the versatility and efficacy of L3Ms in achieving tailored alignments for various applications.

Reward를 제약 조건으로 건 상황에서 SFT. 그런 의미에서 SFT와 RLHF를 통합했다고 표현하고 있네요.

<english>
Doing SFT with reward constraints. It unifies SFT and RLHF in that sense.
</english>

#reward-model #alignment 