https://cdn.openai.com/pdf/34f2ada6-870f-4c26-9790-fd8def56387f/CoT_Monitoring.pdf

*Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation* (Bowen Baker, Joost Huizinga, Leo Gao, Zehao Dou, Melody Y. Guan, Aleksander Madry, Wojciech Zaremba, Jakub Pachocki, David Farhi)

> Mitigating reward hacking—where AI systems misbehave due to flaws or misspecifications in their learning objectives—remains a key challenge in constructing capable and aligned models. We show that we can monitor a frontier reasoning model, such as OpenAI o3-mini, for reward hacking in agentic coding environments by using another LLM that observes the model’s chain-of-thought (CoT) reasoning. CoT monitoring can be far more effective than monitoring agent actions and outputs alone, and we further found that a LLM weaker than o3-mini, namely GPT-4o, can effectively monitor a stronger model. Because CoT monitors can be effective at detecting exploits, it is natural to ask whether those exploits can be suppressed by incorporating a CoT monitor directly into the agent’s training objective. While we show that integrating CoT monitors into the reinforcement learning reward can indeed produce more capable and more aligned agents in the low optimization regime, we find that with too much optimization, agents learn obfuscated reward hacking, hiding their intent within the CoT while still exhibiting a significant rate of reward hacking. Because it is difficult to tell when CoTs have become obfuscated, it may be necessary to pay a monitorability tax by not applying strong optimization pressures directly to the chain-of-thought, ensuring that CoTs remain monitorable and useful for detecting misaligned behavior.

추론 모델의 Reward Hacking을 CoT를 관찰하는 것으로 탐지할 수 있다는 연구. 그렇다면 CoT에 대한 관찰 결과를 토대로 Reward를 준다면 어떨까? 제한된 조건에서긴 하지만 CoT를 위장하는 Reward Hacking이 일어난다고 합니다. 따라서 CoT에는 일단 손대지 않는 것이 좋겠다는 결론.

추가적으로 CoT에서 모델이 자신이 학습 중 혹은 평가 중이라는 것을 인식하는 경우가 있었다고 합니다. Anthropic에서도 연구한 주제죠. (https://arxiv.org/abs/2412.14093) 안전 연구자들이 우려하던 현상들이 보다 현실적인 시나리오에서 실제로 일어나기 시작하네요.

<english>
A study insists it is possible to find out reward hacking of reward models by observing its CoT. Then what if we give a reward based on the observation of CoT? Though it is restricted conditions, the study says that reward hacking of obfuscates CoT occurs. So conclusion is it would be better to not touch CoT.

Additionally, there was a case of model recognizes it is on training or evaluation inside of CoT. It is similar problem Anthropic also studied  (https://arxiv.org/abs/2412.14093). Phenomenon that safety researchers have worried actually happening in more realistic scenarios.
</english>

#reasoning #rl #safety #reward 