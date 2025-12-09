https://arxiv.org/abs/2512.07783

*On the Interplay of Pre-Training, Mid-Training, and RL on Reasoning Language Models* (Charlie Zhang, Graham Neubig, Xiang Yue)

> Recent reinforcement learning (RL) techniques have yielded impressive reasoning improvements in language models, yet it remains unclear whether post-training truly extends a model's reasoning ability beyond what it acquires during pre-training. A central challenge is the lack of control in modern training pipelines: large-scale pre-training corpora are opaque, mid-training is often underexamined, and RL objectives interact with unknown prior knowledge in complex ways. To resolve this ambiguity, we develop a fully controlled experimental framework that isolates the causal contributions of pre-training, mid-training, and RL-based post-training. Our approach employs synthetic reasoning tasks with explicit atomic operations, parseable step-by-step reasoning traces, and systematic manipulation of training distributions. We evaluate models along two axes: extrapolative generalization to more complex compositions and contextual generalization across surface contexts. Using this framework, we reconcile competing views on RL's effectiveness. We show that: 1) RL produces true capability gains (pass@128) only when pre-training leaves sufficient headroom and when RL data target the model's edge of competence, tasks at the boundary that are difficult but not yet out of reach. 2) Contextual generalization requires minimal yet sufficient pre-training exposure, after which RL can reliably transfer. 3) Mid-training significantly enhances performance under fixed compute compared with RL only, demonstrating its central but underexplored role in training pipelines. 4) Process-level rewards reduce reward hacking and improve reasoning fidelity. Together, these results clarify the interplay between pre-training, mid-training, and RL, offering a foundation for understanding and improving reasoning LM training strategies.

프리/미드/포스트트레이닝의 상호작용에 대한 아주 흥미로운 관찰.

1. RL을 통한 성능 향상은 과제가 너무 쉽지도 너무 어렵지도 않을 때 가장 큼.
2. 프리트레이닝은 더 넓은 범위의 Atomic Skill을 함양하는데 집중해야함. 이 Atomic Skill을 결합해 복합 문제를 푸는 것은 RL이 할 수 있음.
3. 프리트레이닝 분포 근처의 과제들에 대해서는 미드트레이닝에 투자하는 것이 효과적. 그러나 더 어려운 과제에 대해서는 RL에 연산력을 더 투입하는 것이 효과적.
4. Process Reward는 일반화에 도움이 됨. (물론 Process Reward를 쓸 수 있는 경우 한정이지만.)

일반 추론에 대해서 Atomic Skill을 어떻게 정의할 것인가? 그리고 Atomic Skill을 어떻게, 특히 합성 데이터를 사용해서, 함양할 수 있을 것인가? RL에 대한 Atomic vs Composite Skill이라는 관점에서 흥미로운 주제일 것.

Very interesting observations on the interaction between pre/mid/post-training.

1. The gain from RL is largest when the task is neither too easy nor too hard.
2. Pretraining should focus on cultivating broader atomic skills - RL can combine them to solve composite problems.
3. For tasks near the pretraining distribution heavy mid-training is effective. For harder tasks assigning more compute to RL is effective.
4. Process rewards are helpful for generalization (if we can utilize them!)

How can we define atomic skills in general reasoning? And how can we further promote that, potentially using synthetic data? This could be an interesting area to explore in the atomic vs composite skills view of RL.

#rl #pretraining #post-training #mid-training 