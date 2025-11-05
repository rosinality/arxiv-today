https://arxiv.org/abs/2511.00413

*Tree Training: Accelerating Agentic LLMs Training via Shared Prefix Reuse* (Shaojie Wang, Jinghui Wang, Yinghan Cui, Xuxing Chen, Chao Wang, Liang Huang, Xiaojiang Zhang, Junyi Peng, Li Wan, Haotian Zhang, Bin Chen)

> In agentic LLM scenarios, an agent's interaction process during a single rollout often exhibits branching behaviors. Due to memory retrieval and concurrent tool executions at certain decision points, the token trajectory of one task evolves into a tree-like structure rather than a linear sequence. However, current training pipelines decompose such tree-structured trajectories into separate linear segments, treating each branch as an independent sequence. As a result, shared prefixes across these branches are repeatedly recomputed during both forward and backward passes. To address this inefficiency, we propose Tree Training, a paradigm that computes each shared prefix only once and reuses its intermediate results across related branches during both forward and backward passes, substantially improving computation efficiency in large-scale agentic training. This is achieved via (i) Tree Packing, which efficiently reuses shared computations across trajectories, and (ii) Gradient Restoration, which ensures correct gradient propagation across reused prefixes. Experiments on multiple open-source models demonstrate up to 3.9x reduction in total training time, enabling more efficient agentic LLM SFT and RL training.

트리 구조의 궤적을 패킹하고 공유되는 Prefix에 대해 중복되는 Forward/Backward 연산을 제거.

Packs tree-structured trajectories and removes redundant forward & backward computations for shared prefixes.

#agent  #efficiency 