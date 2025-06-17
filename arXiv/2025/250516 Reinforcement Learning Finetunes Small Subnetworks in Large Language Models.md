https://arxiv.org/abs/2505.11711

*Reinforcement Learning Finetunes Small Subnetworks in Large Language Models* (Sagnik Mukherjee, Lifan Yuan, Dilek Hakkani-Tur, Hao Peng)

> Reinforcement learning (RL) yields substantial improvements in large language models (LLMs) downstream task performance and alignment with human values. Surprisingly, such large gains result from updating only a small subnetwork comprising just 5 percent to 30 percent of the parameters, with the rest effectively unchanged. We refer to this phenomenon as parameter update sparsity induced by RL. It is observed across all 7 widely used RL algorithms (e.g., PPO, GRPO, DPO) and all 10 LLMs from different families in our experiments. This sparsity is intrinsic and occurs without any explicit sparsity promoting regularizations or architectural constraints. Finetuning the subnetwork alone recovers the test accuracy, and, remarkably, produces a model nearly identical to the one obtained via full finetuning. The subnetworks from different random seeds, training data, and even RL algorithms show substantially greater overlap than expected by chance. Our analysis suggests that this sparsity is not due to updating only a subset of layers, instead, nearly all parameter matrices receive similarly sparse updates. Moreover, the updates to almost all parameter matrices are nearly full-rank, suggesting RL updates a small subset of parameters that nevertheless span almost the full subspaces that the parameter matrices can represent. We conjecture that the this update sparsity can be primarily attributed to training on data that is near the policy distribution, techniques that encourage the policy to remain close to the pretrained model, such as the KL regularization and gradient clipping, have limited impact.

RL 학습 과정에서 Full Rank이지만 SFT에 비해 상당히 희소한 업데이트가 일어난다고 하네요. KL Penalty 등과는 별개로 In-distribution 데이터에 의한 학습의 효과라고. 자연스럽지만 흥미롭군요.

<english>
The study says that although full-rank, but highly sparse update is occur during RL, compared to SFT. It is mainly effect from in-distribution training, rather than KL penalty. It would be natural result but interesting.
</english>

#rl #optimizer #llm 