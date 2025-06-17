https://arxiv.org/abs/2502.01456

*Process Reinforcement through Implicit Rewards* (Ganqu Cui, Lifan Yuan, Zefan Wang, Hanbin Wang, Wendi Li, Bingxiang He, Yuchen Fan, Tianyu Yu, Qixin Xu, Weize Chen, Jiarui Yuan, Huayu Chen, Kaiyan Zhang, Xingtai Lv, Shuo Wang, Yuan Yao, Xu Han, Hao Peng, Yu Cheng, Zhiyuan Liu, Maosong Sun, Bowen Zhou, Ning Ding)

> Dense process rewards have proven a more effective alternative to the sparse outcome-level rewards in the inference-time scaling of large language models (LLMs), particularly in tasks requiring complex multi-step reasoning. While dense rewards also offer an appealing choice for the reinforcement learning (RL) of LLMs since their fine-grained rewards have the potential to address some inherent issues of outcome rewards, such as training efficiency and credit assignment, this potential remains largely unrealized. This can be primarily attributed to the challenges of training process reward models (PRMs) online, where collecting high-quality process labels is prohibitively expensive, making them particularly vulnerable to reward hacking. To address these challenges, we propose PRIME (Process Reinforcement through IMplicit rEwards), which enables online PRM updates using only policy rollouts and outcome labels through implict process rewards. PRIME combines well with various advantage functions and forgoes the dedicated reward model training phrase that existing approaches require, substantially reducing the development overhead. We demonstrate PRIME's effectiveness on competitional math and coding. Starting from Qwen2.5-Math-7B-Base, PRIME achieves a 15.1% average improvement across several key reasoning benchmarks over the SFT model. Notably, our resulting model, Eurus-2-7B-PRIME, surpasses Qwen2.5-Math-7B-Instruct on seven reasoning benchmarks with 10% of its training data.

Implicit PRM으로 학습하는 프로젝트 PRIME에 대한 리포트. (https://arxiv.org/abs/2412.01981) Implicit PRM은 Online 학습이 가능하니 Reward Hacking을 막을 수 있다는 것이 핵심입니다.

실수도 고칠 수 있다면 문제가 아니라고들 하죠. 그런 의미에서는 실수에 대해 Implicit PRM이 어떤 Reward를 부여할지 궁금하네요.

<english>
Report on project (PRIME) which trains a model with implicit PRM. (https://arxiv.org/abs/2412.01981) The main point is it is possible to avoid reward hacking as we can do online training for implicit PRM.

It is commonly said that mistakes are okay if model can fix it after. In that aspect I wonder how implicit PRM sets rewards for mistakes.
</english>

#reward-model #reasoning #rl

# Links

[[241202 Free Process Rewards without Process Labels.md]]