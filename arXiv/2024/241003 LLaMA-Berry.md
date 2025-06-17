https://arxiv.org/abs/2410.02884

*LLaMA-Berry: Pairwise Optimization for O1-like Olympiad-Level Mathematical Reasoning* (Di Zhang, Jianbo Wu, Jingdi Lei, Tong Che, Jiatong Li, Tong Xie, Xiaoshui Huang, Shufei Zhang, Marco Pavone, Yuqiang Li, Wanli Ouyang, Dongzhan Zhou)

> This paper presents an advanced mathematical problem-solving framework, LLaMA-Berry, for enhancing the mathematical reasoning ability of Large Language Models (LLMs). The framework combines Monte Carlo Tree Search (MCTS) with iterative Self-Refine to optimize the reasoning path and utilizes a pairwise reward model to evaluate different paths globally. By leveraging the self-critic and rewriting capabilities of LLMs, Self-Refine applied to MCTS (SR-MCTS) overcomes the inefficiencies and limitations of conventional step-wise and greedy search algorithms by fostering a more efficient exploration of solution spaces. Pairwise Preference Reward Model~(PPRM), inspired by Reinforcement Learning from Human Feedback (RLHF), is then used to model pairwise preferences between solutions, utilizing an Enhanced Borda Count (EBC) method to synthesize these preferences into a global ranking score to find better answers. This approach addresses the challenges of scoring variability and non-independent distributions in mathematical reasoning tasks. The framework has been tested on general and advanced benchmarks, showing superior performance in terms of search efficiency and problem-solving capability compared to existing methods like ToT and rStar, particularly in complex Olympiad-level benchmarks, including GPQA, AIME24 and AMC23.

MCTS + Self-Refine + Pairwise RM. Pairwise RM은 PRM800K와 OpenMathInstruct-1으로 학습되었습니다. 앞으로 Reasoning에 대한 연구들이 쏟아질 텐데 그 중에서 좋은 접근을 발견할 수 있는 취향이 중요해질 것 같네요.

<english>
MCTS + Self-Refine + Pairwise RM. Pairwise RM is trained with PRM800K and OpenMathInstruct-1. Vast amount of papers around the reasoning problem will appear, and it will be important to have tastes that allow one to find out good approaches.
</english>

#search #mcts 