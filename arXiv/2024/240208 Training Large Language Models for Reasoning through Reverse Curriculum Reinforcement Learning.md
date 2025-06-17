https://arxiv.org/abs/2402.05808

*Training Large Language Models for Reasoning through Reverse Curriculum Reinforcement Learning* (Zhiheng Xi, Wenxiang Chen, Boyang Hong, Senjie Jin, Rui Zheng, Wei He, Yiwen Ding, Shichun Liu, Xin Guo, Junzhe Wang, Honglin Guo, Wei Shen, Xiaoran Fan, Yuhao Zhou, Shihan Dou, Xiao Wang, Xinbo Zhang, Peng Sun, Tao Gui, Qi Zhang, Xuanjing Huang)

> In this paper, we propose R$^3$: Learning Reasoning through Reverse Curriculum Reinforcement Learning (RL), a novel method that employs only outcome supervision to achieve the benefits of process supervision for large language models. The core challenge in applying RL to complex reasoning is to identify a sequence of actions that result in positive rewards and provide appropriate supervision for optimization. Outcome supervision provides sparse rewards for final results without identifying error locations, whereas process supervision offers step-wise rewards but requires extensive manual annotation. R$^3$ overcomes these limitations by learning from correct demonstrations. Specifically, R$^3$ progressively slides the start state of reasoning from a demonstration's end to its beginning, facilitating easier model exploration at all stages. Thus, R$^3$ establishes a step-wise curriculum, allowing outcome supervision to offer step-level signals and precisely pinpoint errors. Using Llama2-7B, our method surpasses RL baseline on eight reasoning tasks by $4.1$ points on average. Notebaly, in program-based reasoning on GSM8K, it exceeds the baseline by $4.2$ points across three backbone models, and without any extra data, Codellama-7B + R$^3$ performs comparable to larger models or closed-source models.

Outcome supervision의 저렴하지만 학습 시그널이 줄어드는 문제, Process supervision의 학습 시그널이 늘어나지만 데이터 구축 비용이 높아지는 문제를 절충하려고 시도한 방법.

기본적으로 Golden reasoning chain 데이터가 있다고 가정하고 시작합니다. Reasoning chain을 나눠서 마지막 스텝만 예측하기, 끝에서 두 개 스텝을 예측하기 등등으로 전체를 예측하는 것이 아니라 일부만 예측하게 하는 방법으로 가이드를 준다고 할 수 있겠네요.

#reward-model 

Outcome supervision is inexpensive but has sparse supervision signals. Process supervision has dense supervision signals but its annotation cost is expensive. This study targets to combine pros of outcome supervision and process supervision.

Basically it assumes we have golden reasoning chain examples. Then by splitting reasoning chains, it makes models to final reasoning steps, or from penultimate steps to final steps, and so on, that is, instead of predict all of the reasoning steps, it guides model to partially predict reasoning steps conditioned on previous steps.