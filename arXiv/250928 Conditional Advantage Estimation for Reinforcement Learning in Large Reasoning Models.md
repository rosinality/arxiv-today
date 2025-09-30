https://arxiv.org/abs/2509.23962

*Conditional Advantage Estimation for Reinforcement Learning in Large Reasoning Models* (Guanxu Chen, Yafu Li, Yuxian Jiang, Chen Qian, Qihan Ren, Jingyi Yang, Yu Cheng, Dongrui Liu, Jing Shao)

> Reinforcement Learning with Verifiable Rewards (RLVR) for large language models (LLMs) has achieved remarkable progress in enhancing LLMs' reasoning capabilities on tasks with clear correctness criteria, such as mathematical reasoning tasks. Several training metrics, such as entropy or response length, have been observed to correlate with different reasoning behaviors in reinforcement learning. Prior approaches incorporate such priors through reward or advantage shaping, which often relies on hand-crafted penalties and preferences (e.g., higher-is-better or lower-is-better). However, without careful hyperparameter tuning, these directional priors can be overly biased and may lead to failure. To this end, we introduce Conditional advANtage estimatiON (CANON), amplifying the impact of the target metric without presuming its direction. Specifically, CANON regroups the sampled responses into two groups based on the higher or lower value of a target metric, measures which metric trend contributes to better performance through inter-group comparison, and identifies the better response within the same group. In summary, CANON based on entropy consistently outperforms prior methods across three LLMs on both math reasoning and high-complexity logic tasks. When applied to response length, CANON further improves token efficiency, yielding a more favorable Pareto frontier in the performance-cost trade-off.

<english>
Makes subgroup of samples according to desired conditions and adjust advantages usi

#rl #reasoning 