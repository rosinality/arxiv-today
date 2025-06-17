https://arxiv.org/abs/2412.01981

*Free Process Rewards without Process Labels* (Lifan Yuan, Wendi Li, Huayu Chen, Ganqu Cui, Ning Ding, Kaiyan Zhang, Bowen Zhou, Zhiyuan Liu, Hao Peng)

> Different from its counterpart outcome reward models (ORMs), which evaluate the entire responses, a process reward model (PRM) scores a reasoning trajectory step by step, providing denser and more fine grained rewards. However, training a PRM requires labels annotated at every intermediate step, presenting significant challenges for both manual and automatic data collection. This paper aims to address this challenge. Both theoretically and empirically, we show that an \textit{implicit PRM} can be obtained at no additional cost, by simply training an ORM on the cheaper response-level labels. The only assumption is to parameterize the outcome reward as the log-likelihood ratios of the policy and reference models, which can be optimized regardless of the specific choice of loss objectives. In experiments, we instantiate our implicit PRMs with various objectives and evaluate their performance on MATH. We show that our implicit PRM outperforms a strong MCTS-based baseline \textit{\'a la} Math-Shepherd using less than $1/38$ of the training data. Its performance can be further improved with majority voting. We further find that scaling up instructions and responses benefits our implicit PRM, and the latter brings a larger gain. Particularly, we find that our implicit PRM, when instantiated with the cross-entropy (CE) loss, is more data-efficient and can keep improving generation models even when trained with only one response per instruction, the setup that suffers from extreme data scarcity and imbalance. Further, instructions should be relevant to downstream tasks while the diversity of responses does not bring gains. Surprisingly, training on extra Math-Shepherd step labels brings no further improvements to our implicit PRM trained on only outcome data. We hope that our work will encourage a rethinking of PRM training approaches and contribute to making training PRMs more accessible.

Policy와 Reference 모델의 log likelihood ratio를 Reward로 Parameterize한 Outcome Reward Model을 통해 Process Reward를 부여할 수 있다는 연구. DPO와 Q의 관계, 토큰 단위 Credit Assignment에 대한 결과의 연장선이라고 할 수 있겠네요.

<english>
The study that we can assign process reward using outcome reward model which parameterizes reward as log likelihood ratio of policy and reference. It is in line of the research on the relationship of DPO and Q, and token level credit assignment. (https://arxiv.org/abs/2404.12358)
</english>

#reward-model

# Links

[[240418 From $r$ to $Q^.md]]