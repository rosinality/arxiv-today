https://arxiv.org/abs/2405.10938

*Observational Scaling Laws and the Predictability of Language Model Performance* (Yangjun Ruan, Chris J. Maddison, Tatsunori Hashimoto)

> Understanding how language model performance varies with scale is critical to benchmark and algorithm development. Scaling laws are one approach to building this understanding, but the requirement of training models across many different scales has limited their use. We propose an alternative, observational approach that bypasses model training and instead builds scaling laws from ~80 publically available models. Building a single scaling law from multiple model families is challenging due to large variations in their training compute efficiencies and capabilities. However, we show that these variations are consistent with a simple, generalized scaling law where language model performance is a function of a low-dimensional capability space, and model families only vary in their efficiency in converting training compute to capabilities. Using this approach, we show the surprising predictability of complex scaling phenomena: we show that several emergent phenomena follow a smooth, sigmoidal behavior and are predictable from small models; we show that the agent performance of models such as GPT-4 can be precisely predicted from simpler non-agentic benchmarks; and we show how to predict the impact of post-training interventions like Chain-of-Thought and Self-Consistency as language model capabilities continue to improve.

벤치마크에 대한 Scaling Law도 많이 발전하고 있네요. 여기서는 벤치마크의 스코어들을 차원 축소한 다음 모델 클래스 (Llama 등) 내에서의 연산량의 증가와 차원 축소해서 추출한 요인 사이의 관계를 사용해서 벤치마크 스코어에 대한 Scaling Law를 만들었네요.

복잡하게 쓰긴 했는데 결국 다층 모형입니다.

가장 흥미로운 것은 각 모델 클래스 내에서 연산량과 요인에 대해 선형적인 관계가 있고 이 직선의 기울기가 연산 효율성을 의미한다는 것입니다. 이 기울기가 낮다면 뭔가 잘못 하고 있다는 의미라는 것이겠죠.

여담이지만 주요 요인은 일반 능력, 추론 능력, 프로그래밍 능력 세 가지로 레이블링을 했는데 이 요인들의 가중치를 보면 가장 중요한 3대 벤치마크는 MMLU, GSM8K, HumanEval이라고 할 수 있을 것 같네요.

#scaling-law 