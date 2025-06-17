https://github.com/deepseek-ai/DeepSeek-R1/blob/main/DeepSeek_R1.pdf

*DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning* (DeepSeek-AI)

> We introduce our first-generation reasoning models, DeepSeek-R1-Zero and DeepSeek-R1. DeepSeek-R1-Zero, a model trained via large-scale reinforcement learning (RL) without super- vised fine-tuning (SFT) as a preliminary step, demonstrates remarkable reasoning capabilities. Through RL, DeepSeek-R1-Zero naturally emerges with numerous powerful and intriguing reasoning behaviors. However, it encounters challenges such as poor readability, and language mixing. To address these issues and further enhance reasoning performance, we introduce DeepSeek-R1, which incorporates multi-stage training and cold-start data before RL. DeepSeek- R1 achieves performance comparable to OpenAI-o1-1217 on reasoning tasks. To support the research community, we open-source DeepSeek-R1-Zero, DeepSeek-R1, and six dense models (1.5B, 7B, 8B, 14B, 32B, 70B) distilled from DeepSeek-R1 based on Qwen and Llama.

DeepSeek의 추론 모델. PRM, ORM, MCTS 등을 전혀 사용하지 않고 규칙(정답) 기반의 Reward로 GRPO를 한 형태입니다. TÜLU 3의 RLVR과 (https://arxiv.org/abs/2411.15124) 비슷합니다. 이를 통해 자신의 생각에 대해 재검토하는 등의 새로운 능력이 등장하는 것을 관찰할 수 있었다고 합니다. (Aha moment, Nathan Lambert가 RLVR에 대해서 Outcome Reward만으로도 새로운 능력을 나타내게 할 수 있다고 언급했는데 이에 대한 사례겠네요. https://www.interconnects.ai/p/openais-o1-using-search-was-a-psyop?utm_source=publication-search)

가장 기본적인 RL만으로 추론 능력을 부여하는 것이 가능하다는 것을 확인한 후 일반화된 모델을 만들기 위한 작업을 했습니다. 우선 CoT 데이터를 조금 사용해 깔끔한 CoT를 생성할 수 있게 한 다음 정답 기반 추론 RL을 진행하고, 기존 SFT 데이터에 추론 데이터, Generative Reward Model로 Rejection Sampling한 데이터를 합쳐 SFT 데이터를 구축하고, 이 위에 RLHF와 추론 RL을 진행했습니다.

그리고 이 SFT 데이터를 통해 작은 모델에 Distill 하는 실험을 했네요. Distill로 추론 능력을 부여할 수 있다는 것은 최근 사례들에서 여러 번 드러났죠. 작은 모델에 대해 RL로 학습하는 것보다 Distill 쪽이 더 나은 결과가 나왔다고 합니다. RL을 통해 더 나은 성능을 얻기 위해서는 베이스 모델의 퀄리티가 뒷받침 되어야 한다는 것을 시사하는 결과겠네요.

Distill 쪽이 훨씬 쉽게 결과를 얻을 수 있기 때문에 지금까지 그랬던 것처럼 앞으로도 이쪽에 대한 관심이 높을 것 같습니다. 그러나 논문에서 지적하듯 더 나아가기 위해선 여전히 더 강력한 베이스 모델과 대규모 RL이 필요하겠죠.

<english>
Reasoning model from DeepSeek. They did not used any of PRM, ORM, MCTS and instead did GRPO with rule (correctness) based rewards. It is similar to RLVR from TÜLU 3 (https://arxiv.org/abs/2411.15124). They reports that it is able to observe the emergence of new abilities like re-evaluates its previous thoughts. (Aha moment, an example that it is possible to make new abilities emerge by only using outcome rewards, which Nathan Lambert mentioned. https://www.interconnects.ai/p/openais-o1-using-search-was-a-psyop?utm_source=publication-search)

After confirm it is able to give reasoning ability by most basic form of RL they did an work for building generalized models. First they have used small amout of CoT data to let model generate clean CoT, and did reasoning RL based on correctness, and built SFT data by combining previous SFT data and rejection sampled data using reasoning correctness or generative reward models, and finally did RLHF and reasoning RL on the model.

And they did an experiment of distillation into small models using these SFT data. Recent studies shown that it is able to give reasoning abilities by distillation. They says that they can get better results for small models from distillation instead of RL. It suggest that it should be backed by strong quality base models to get better results with RL.

As distillation allows much easier way to get a result there will be higher interest on this, just like before. However, as the paper points out, we need more powerful base models and large scale RL to advancing the capability of the model.
</english>


#rl #reasoning 