https://machinelearning.apple.com/papers/apple_intelligence_foundation_language_models.pdf

*Apple Intelligence FoundationLanguage Models* (Apple)

> We present foundation language models developed to power Apple Intelligence features, including a ∼3 billion parameter model designed to run efficiently on devices and a large server-based language model designed for Private Cloud Compute [Apple, 2024b]. These models are designed to perform a wide range of tasks efficiently, accurately, and responsibly. This report describes the model architecture, the data used to train the model, the training process, how the models are optimized for inference, and the evaluation results. We highlight our focus on Responsible AI and how the principles are applied throughout the model development.We present foundation language models developed to power Apple Intelligence features, including a ∼3 billion parameter model designed to run efficiently on devices and a large server-based language model designed for Private Cloud Compute [Apple, 2024b]. These models are designed to perform a wide range of tasks efficiently, accurately, and responsibly. This report describes the model architecture, the data used to train the model, the training process, how the models are optimized for inference, and the evaluation results. We highlight our focus on Responsible AI and how the principles are applied throughout the model development.

애플의 LLM. 온디바이스 모델과 서버 모델로 나뉘는데 온디바이스 모델에 대해서는 크기를 공개했지만(3B) 서버 모델에 대해서는 언급이 없네요.

생각보다 특이한 디테일들이 많이 있습니다. QK Norm을 사용했고 자체 크롤러로 수집한 데이터로 LLM 기반 필터링도 사용했군요. (https://arxiv.org/abs/2406.04638) 수학 데이터 추가 수집을 진행했고 라이선스를 받은 데이터셋을 사용했다는데 이쪽이 Long Context 학습에 들어간 것을 보면 대략 어떤 데이터인지 알 수 있을 것 같네요.

Simple μP를 사용해서 768 dim 모델의 LR을 Transfer 했고 그 결과 LR이 0.1배가 되었다는 언급을 고려하면 서버 모델은 아마 30 - 70B 모델이 아닐까 싶네요. 서버와 온디바이스 모델 모두 6.3T 학습했는데 온디바이스 모델은 6.4B 모델을 프루닝하고 Knowledge Distillation을 했군요. Independent Weight Decay를 사용했고 서버 모델은 배치 크기 추정으로 16M 배치를 사용했습니다. 정확하게는 12M 배치가 최적으로 나왔지만 2배 정도 까지는 큰 문제가 없어서 16M을 사용했다고.

RMSprop + Momentum, eps = 1e-30. 업데이트 자체의 Norm을 1로 제한. TPU를 사용해 학습했습니다.

포스트트레이닝. 수학에 대해서는 Evol Instruct 스타일의 프롬프트 확장. 코딩에 대해서는 Self Instruct 스타일로 프롬프트를 생성하고 Execution Feedback. Llama 2의 Margin Based Loss와는 좀 다르지만 Preference의 강도에 따라 변화하는 Soft Label Loss와 Single Sided Grading Loss.

Human Preference 데이터 수집 과정에서 SFT, Rejection Sampling, DPO/IPO, RL로 학습된 여러 모델들의 샘플에 대해서 어노테이션을 하고 이를 통해 학습한 Reward Model을 이 여러 모델들의 샘플에 적용해서 Rejection Sampling을 하고 이 결과를 사용해 추가 학습. 여러 스타일로 학습된 모델들의 장점을 모으려고 했다고.

RLHF는 PPO 대신 Mirror Descent 기반으로 (https://arxiv.org/abs/2005.09814) Leave One Out Estimator를 (https://arxiv.org/abs/2402.14740) 사용했습니다. 전부 하나씩 다르네요.

Quantization을 상당히 강력하게 하면서 LoRA를 사용해 성능 감소를 커버하는 접근을 썼군요. 평균적으로 Weight 당 3.7 bit를 썼다고 합니다.

#llm 