https://arxiv.org/abs/2403.07708

*Improving Reinforcement Learning from Human Feedback Using Contrastive Rewards* (Wei Shen, Xiaoying Zhang, Yuanshun Yao, Rui Zheng, Hongyi Guo, Yang Liu)

> Reinforcement learning from human feedback (RLHF) is the mainstream paradigm used to align large language models (LLMs) with human preferences. Yet existing RLHF heavily relies on accurate and informative reward models, which are vulnerable and sensitive to noise from various sources, e.g. human labeling errors, making the pipeline fragile. In this work, we improve the effectiveness of the reward model by introducing a penalty term on the reward, named as \textit{contrastive rewards}. %Contrastive rewards Our approach involves two steps: (1) an offline sampling step to obtain responses to prompts that serve as baseline calculation and (2) a contrastive reward calculated using the baseline responses and used in the Proximal Policy Optimization (PPO) step. We show that contrastive rewards enable the LLM to penalize reward uncertainty, improve robustness, encourage improvement over baselines, calibrate according to task difficulty, and reduce variance in PPO. We show empirically contrastive rewards can improve RLHF substantially, evaluated by both GPTs and humans, and our method consistently outperforms strong baselines.

SFT 모델로 샘플을 여러 개 뽑은 다음 Reward 스코어의 평균을 내서 PPO 시점에 샘플의 Reward에서 이 평균을 뺀 값을 Reward로 사용한다는 아이디어. 샘플을 여러 개 생성 - 이 샘플들의 스코어를 사용이라고 하는 최근 많이 나오는 패턴이죠.

#rlhf 