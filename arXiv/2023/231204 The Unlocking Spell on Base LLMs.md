https://arxiv.org/abs/2312.01552

The Unlocking Spell on Base LLMs: Rethinking Alignment via In-Context Learning (Bill Yuchen Lin, Abhilasha Ravichander, Ximing Lu, Nouha Dziri, Melanie Sclar, Khyathi Chandu, Chandra Bhagavatula, Yejin Choi)

정렬된 모델과 베이스 모델의 토큰 확률 차이를 보니 주로 응답 스타일과 관련된 토큰들에서 변화가 컸다고 하네요. 반대로 정보와 관련된 토큰에서는 차이가 작았다고 합니다. LIMA에서 시작된 (https://arxiv.org/abs/2305.11206) Alignment 튜닝은 스타일을 보정하는 것일 뿐이라는 계통의 결과입니다.

그러니 In-context learning으로도 풀 수 있지 않을까? 하는 생각으로 시스템 프롬프트와 ChatGPT 스타일의 응답 3개로 프롬프트를 만들어 테스트해봤습니다. 결과적으로 꽤 잘 된다는 것을 발견했습니다.

In-context learning으로 일단 대화가 되게 만들고 그 위에 RLHF를 올린다는 발상은 Anthropic (https://arxiv.org/abs/2204.05862) 이나 SALMON (https://arxiv.org/abs/2310.05910) 에서도 발견할 수 있는 결과죠. 다만 현재 오픈소스 LLM들의 주요 전략인 필터링된 GPT-4 응답을 충분히 많이 집어넣는다와는 결이 다릅니다. 전 FLAN 류의 Instruction following 데이터셋을 프리트레이닝에 첨가하면 In-context learning 수준에서도 꽤 괜찮은 수준이 가능하지 않을까 하는 생각이 있습니다.

#alignment 

[[230518 LIMA]]
[[230629 Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback]]
[[231009 SALMON]]

# Links

[[230518 LIMA.md]]
[[230629 Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback]]