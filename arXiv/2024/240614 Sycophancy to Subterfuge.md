https://arxiv.org/abs/2406.10162

*Sycophancy to Subterfuge: Investigating Reward-Tampering in Large Language Models* (Carson Denison, Monte MacDiarmid, Fazl Barez, David Duvenaud, Shauna Kravec, Samuel Marks, Nicholas Schiefer, Ryan Soklaski, Alex Tamkin, Jared Kaplan, Buck Shlegeris, Samuel R. Bowman, Ethan Perez, Evan Hubinger)

> In reinforcement learning, specification gaming occurs when AI systems learn undesired behaviors that are highly rewarded due to misspecified training goals. Specification gaming can range from simple behaviors like sycophancy to sophisticated and pernicious behaviors like reward-tampering, where a model directly modifies its own reward mechanism. However, these more pernicious behaviors may be too complex to be discovered via exploration. In this paper, we study whether Large Language Model (LLM) assistants which find easily discovered forms of specification gaming will generalize to perform rarer and more blatant forms, up to and including reward-tampering. We construct a curriculum of increasingly sophisticated gameable environments and find that training on early-curriculum environments leads to more specification gaming on remaining environments. Strikingly, a small but non-negligible proportion of the time, LLM assistants trained on the full curriculum generalize zero-shot to directly rewriting their own reward function. Retraining an LLM not to game early-curriculum environments mitigates, but does not eliminate, reward-tampering in later environments. Moreover, adding harmlessness training to our gameable environments does not prevent reward-tampering. These results demonstrate that LLMs can generalize from common forms of specification gaming to more pernicious reward tampering and that such behavior may be nontrivial to remove.

상당히 복잡하면서도 Anthropic스러운 SF 같은 세팅의 연구입니다. 여기서 다루는 것은 Specification gaming 문제입니다. RL에서 종종 일어나는 요구 조건은 충족하지만 의도한 목적이 아니라 다른 방식으로 조건을 충족하는 문제죠.

여기서 Specification gaming이 일어났을 때 좀 더 단순하고 캐주얼한 문제에 대해 일어난 Gaming 패턴이 더 중요한 문제에 대해서도 Gaming을 하는 것으로 일반화가 될 수 있는지가 연구의 주요 문제입니다. 예를 들어 단순한 문제에 대해서 Gaming을 학습한 모델이 모델 자신의 학습 코드를 이상하게 고친다거나 하는 가능성이 있을까 하는 것이죠.

연구 세팅에서는 Sycophancy (https://arxiv.org/abs/2310.13548) 같은 문제를 유도한 모델에게 모델에 대한 RL이 얼마나 진행되었는가 같은 지시를 주었을 때 코드와 테스트를 조작하는 행동을 할 수 있는가를 분석했습니다.

결과적으로 확률이 낮기는 한데 (1/1000) 이런 일반화가 일어날 수 있다는 결론입니다. Claude 2로 실험한 결과이기에 더 강력한 모델을 사용한다면 더더욱 더 가능하지 않을까 하는 이야기를 하고 있네요.

#safety #alignment

# Links

[[231020 Towards Understanding Sycophancy in Language Models.md]]