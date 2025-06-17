https://arxiv.org/abs/2408.11791

*Critique-out-Loud Reward Models* (Zachary Ankner, Mansheej Paul, Brandon Cui, Jonathan D. Chang, Prithviraj Ammanabrolu)

> Traditionally, reward models used for reinforcement learning from human feedback (RLHF) are trained to directly predict preference scores without leveraging the generation capabilities of the underlying large language model (LLM). This limits the capabilities of reward models as they must reason implicitly about the quality of a response, i.e., preference modeling must be performed in a single forward pass through the model. To enable reward models to reason explicitly about the quality of a response, we introduce Critique-out-Loud (CLoud) reward models. CLoud reward models operate by first generating a natural language critique of the assistant's response that is then used to predict a scalar reward for the quality of the response. We demonstrate the success of CLoud reward models for both Llama-3-8B and 70B base models: compared to classic reward models CLoud reward models improve pairwise preference classification accuracy on RewardBench by 4.65 and 5.84 percentage points for the 8B and 70B base models respectively. Furthermore, CLoud reward models lead to a Pareto improvement for win rate on ArenaHard when used as the scoring model for Best-of-N. Finally, we explore how to exploit the dynamic inference compute capabilities of CLoud reward models by performing self-consistency decoding for reward prediction.

SFT로 Critique 생성을 학습시킨 Reward Model. Critique 결합은 한동안 많이 나왔었죠. 거기에 추론 시점에 Self Consistency를 시도. Policy만큼 Reward Model 추론에 연산을 써야 하긴 하네요.

생각해보면 Preference Pair도 정답이 있는 데이터이니 ReST 스타일 학습이 가능할지도 모르겠네요.

#reward-model 