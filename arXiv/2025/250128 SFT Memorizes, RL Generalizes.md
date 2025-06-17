https://arxiv.org/abs/2501.17161

*SFT Memorizes, RL Generalizes: A Comparative Study of Foundation Model Post-training* (Tianzhe Chu, Yuexiang Zhai, Jihan Yang, Shengbang Tong, Saining Xie, Dale Schuurmans, Quoc V. Le, Sergey Levine, Yi Ma)

> Supervised fine-tuning (SFT) and reinforcement learning (RL) are widely used post-training techniques for foundation models. However, their roles in enhancing model generalization capabilities remain unclear. This paper studies the difference between SFT and RL on generalization and memorization, focusing on text-based rule variants and visual variants. We introduce GeneralPoints, an arithmetic reasoning card game, and adopt V-IRL, a real-world navigation environment, to assess how models trained with SFT and RL generalize to unseen variants in both textual and visual domains. We show that RL, especially when trained with an outcome-based reward, generalizes across both rule-based textual and visual variants. SFT, in contrast, tends to memorize training data and struggles to generalize out-of-distribution scenarios. Further analysis reveals that RL improves the model's underlying visual recognition capabilities, contributing to its enhanced generalization in the visual domain. Despite RL's superior generalization, we show that SFT remains essential for effective RL training; SFT stabilizes the model's output format, enabling subsequent RL to achieve its performance gains. These findings demonstrates the capability of RL for acquiring generalizable knowledge in complex, multi-modal tasks.

Outcome Reward 기반 RL로 학습시켰을 때 SFT와는 달리 OOD에 대한 일반화가 일어난다는 연구. 이쪽의 RL 세팅은 Revision과 Verification이 포함된 형태라 아주 기본적인 세팅은 아닙니다.

Revision은 꽤 흥미로운 접근이라는 생각을 합니다. (https://arxiv.org/abs/2409.12917)

In contrast to SFT, RL is able to generalize to OOD when trained with outcome rewards. But it is not very "basic" RL as it includes revision and verification.

I think revision is quite interesting approach. (https://arxiv.org/abs/2409.12917)

#rl #generalization

# Links

[[240919 Training Language Models to Self-Correct via Reinforcement Learning.md]]