https://arxiv.org/abs/2508.07534

*From Trial-and-Error to Improvement: A Systematic Analysis of LLM Exploration Mechanisms in RLVR* (Jia Deng, Jie Chen, Zhipeng Chen, Daixuan Cheng, Fei Bai, Beichen Zhang, Yinqian Min, Yanzipeng Gao, Wayne Xin Zhao, Ji-Rong Wen)

> Reinforcement learning with verifiable rewards (RLVR) has emerged as a powerful paradigm for enhancing the reasoning capabilities of large language models (LLMs). Unlike traditional RL approaches, RLVR leverages rule-based feedback to guide LLMs in generating and refining complex reasoning chains -- a process critically dependent on effective exploration strategies. While prior work has demonstrated RLVR's empirical success, the fundamental mechanisms governing LLMs' exploration behaviors remain underexplored. This technical report presents a systematic investigation of exploration capacities in RLVR, covering four main aspects: (1) exploration space shaping, where we develop quantitative metrics to characterize LLMs' capability boundaries; (2) entropy-performance exchange, analyzed across training stages, individual instances, and token-level patterns; and (3) RL performance optimization, examining methods to effectively translate exploration gains into measurable improvements. By unifying previously identified insights with new empirical evidence, this work aims to provide a foundational framework for advancing RLVR systems.

추론 RL의 엔트로피 측면에 대한 분석. Pass@k를 유지시키는 방법을 찾는다는 방향을 향하는데 어쩌면 그런 의미에서 Pass@k를 직접 노리는 것이 좋은 방향일 수 있을 것 (https://arxiv.org/abs/2508.10751). 

Analysis of the entropy aspect of reasoning RL. They tried to find methods that preserve pass@k, and in that sense, it might be a good approach to directly target pass@k (https://arxiv.org/abs/2508.10751).

#rl #reasoning 