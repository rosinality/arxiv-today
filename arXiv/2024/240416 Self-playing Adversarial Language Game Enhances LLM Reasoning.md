https://arxiv.org/abs/2404.10642

*Self-playing Adversarial Language Game Enhances LLM Reasoning* (Pengyu Cheng, Tianhao Hu, Han Xu, Zhisong Zhang, Yong Dai, Lei Han, Nan Du)

> We explore the self-play training procedure of large language models (LLMs) in a two-player adversarial language game called Adversarial Taboo. In this game, an attacker and a defender communicate with respect to a target word only visible to the attacker. The attacker aims to induce the defender to utter the target word unconsciously, while the defender tries to infer the target word from the attacker's utterances. To win the game, both players should have sufficient knowledge about the target word and high-level reasoning ability to infer and express in this information-reserved conversation. Hence, we are curious about whether LLMs' reasoning ability can be further enhanced by Self-Play in this Adversarial language Game (SPAG). With this goal, we let LLMs act as the attacker and play with a copy of itself as the defender on an extensive range of target words. Through reinforcement learning on the game outcomes, we observe that the LLMs' performance uniformly improves on a broad range of reasoning benchmarks. Furthermore, iteratively adopting this self-play process can continuously promote LLM's reasoning ability. The code is at https://github.com/Linear95/SPAG.

단어 하나를 주고 공격자는 그 단어를 말하지 않으면서 방어자가 자기도 모르게 말하게 하도록 하고 방어자는 그 단어를 맞히는 게임 (https://arxiv.org/abs/1911.01622) 을 사용해 RL을 하는 것으로 추론 능력을 향상시킬 수 있다는 결과.

이런 게임에서 습득한 능력이 다른 과제로 일반화 될 수 있다는 것이 흥미롭네요. RL을 위한 Reward를 설정하는 것이 문제였는데 다소간 인위적인 과제라도 그것이 다른 과제에 대한 향상으로 이어질 수 있다면 그것도 한 가지 방향이 되겠죠.

#rl #llm

# Links

