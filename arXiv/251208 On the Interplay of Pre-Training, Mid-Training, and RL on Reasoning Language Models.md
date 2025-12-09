https://arxiv.org/abs/2512.07783

*On the Interplay of Pre-Training, Mid-Training, and RL on Reasoning Language Models* (Charlie Zhang, Graham Neubig, Xiang Yue)

> Recent reinforcement learning (RL) techniques have yielded impressive reasoning improvements in language models, yet it remains unclear whether post-training truly extends a model's reasoning ability beyond what it acquires during pre-training. A central challenge is the lack of control in modern training pipelines: large-scale pre-training corpora are opaque, mid-training is often underexamined, and RL objectives interact with unknown prior knowledge in complex ways. To resolve this ambiguity, we develop a fully controlled experimental framework that isolates the causal contributions of pre-training, mid-training, and RL-based post-training. Our approach employs synthetic reasoning tasks with explicit atomic operations, parseable step-by-step reasoning traces, and systematic manipulation of training distributions. We evaluate models along two axes: extrapolative generalization to more complex compositions and contextual generalization across surface contexts. Using this framework, we reconcile competing views on RL's effectiveness. We show that: 1) RL produces true capability gains (pass@128) only when pre-training leaves sufficient headroom and when RL data target the model's edge of competence, tasks at the boundary that are difficult but not yet out of reach. 2) Contextual generalization requires minimal yet sufficient pre-training exposure, after which RL can reliably transfer. 3) Mid-training significantly enhances performance under fixed compute compared with RL only, demonstrating its central but underexplored role in training pipelines. 4) Process-level rewards reduce reward hacking and improve reasoning fidelity. Together, these results clarify the interplay between pre-training, mid-training, and RL, offering a foundation for understanding and improving reasoning LM training strategies.

Very interesting observations on the interaction between pre/mid/post-training.

1. The gain from RL is largest when the task is neither too easy nor too hard.
2. Pretraining should focus on cultivating broader atomic skills - RL can combine them to solve composite problems.
3. For tasks near the pretraining distribution heavy mid-training is effective. For harder tasks assigning more compute to RL is effective.
4. Process rewards are helpful for generalization (if we can utilize them!)

How can we define atomic skills in general reasoning? And how can we further promote that, potentially using synthetic data? This could be an interesting area to explore in the atomic vs composite skills view of RL.

#rl #pretraining #post-training #mid-training 