https://arxiv.org/abs/2402.14740

*Back to Basics: Revisiting REINFORCE Style Optimization for Learning from Human Feedback in LLMs* (Arash Ahmadian, Chris Cremer, Matthias Gallé, Marzieh Fadaee, Julia Kreutzer, Ahmet Üstün, Sara Hooker)

> AI alignment in the shape of Reinforcement Learning from Human Feedback (RLHF) is increasingly treated as a crucial ingredient for high performance large language models. \textsc{Proximal Policy Optimization} (PPO) has been positioned by recent literature as the canonical method for the RL part of RLHF. However, it involves both high computational cost and sensitive hyperparameter tuning. We posit that most of the motivational principles that led to the development of PPO are less of a practical concern in RLHF and advocate for a less computationally expensive method that preserves and even increases performance. We revisit the \textit{formulation} of alignment from human preferences in the context of RL. Keeping simplicity as a guiding principle, we show that many components of PPO are unnecessary in an RLHF context and that far simpler REINFORCE-style optimization variants outperform both PPO and newly proposed "RL-free" methods such as DPO and RAFT. Our work suggests that careful adaptation to LLMs alignment characteristics enables benefiting from online RL optimization at low cost.

구글에 이어 PPO를 벗어난 사례가 등장했군요. REINFORCE에 N개 샘플을 사용해 베이스라인을 계산하는 RLOO를 시도했습니다. N개 샘플을 사용하는 시도가 최근 많이 등장하네요.

#rlhf 