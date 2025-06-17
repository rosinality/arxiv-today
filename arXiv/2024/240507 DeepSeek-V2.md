https://github.com/deepseek-ai/DeepSeek-V2/blob/main/deepseek-v2-tech-report.pdf

*DeepSeek-V2: A Strong, Economical, and Efficient Mixture-of-Experts Language Model* (DeepSeek-AI)

> We present DeepSeek-V2, a strong Mixture-of-Experts (MoE) language model characterized by economical training and efficient inference. It comprises 236B total parameters, of which 21B are activated for each token, and supports a context length of 128K tokens. DeepSeek-V2 adopts innovative architectures including Multi-head Latent Attention (MLA) and DeepSeekMoE. MLA guarantees efficient inference through significantly compressing the Key-Value (KV) cache into a latent vector, while DeepSeekMoE enables training strong models at an economical cost through sparse computation. Compared with DeepSeek 67B, DeepSeek-V2 achieves significantly stronger performance, and meanwhile saves 42.5% of training costs, reduces the KV cache by 93.3%, and boosts the maximum generation throughput to 5.76 times. We pretrain DeepSeek-V2 on a high-quality and multi-source corpus consisting of 8.1T tokens, and further perform Supervised Fine-Tuning (SFT) and Reinforcement Learning (RL) to fully unlock its potential. Evaluation results show that, even with only 21B activated parameters, DeepSeek-V2 and its chat versions still achieve top-tier performance among open-source models. The model checkpoints are available at https://github.com/deepseek-ai/DeepSeek-V2.

DeepSeek의 21B Activated / 236B Total Parameter, 8.1T 학습 MoE 모델. GQA나 MQA 대신 Key/Value를 Down Projection 한 다음 Up Projection을 다시 하는 방법을 썼네요. 성능 문제 때문이었다고 하는데 이쪽은 생각을 해봐야 할 것 같습니다.

MoE는 DeepSeek MoE의 세팅과 유사하게 2개의 공유 Expert, 160개의 Expert 중에서 6개의 Expert로 라우팅하는 형태입니다. 여러 개 Expert에 대해 라우팅하면서 발생하는 통신 문제 억제를 위해 최대 M개 디바이스의 Expert에 대해서만 라우팅하도록 하는 밸런싱이 들어갔습니다.

DeepSeek는 늘 일반적인 선택과는 조금씩 다른 선택을 하고 있네요.

데이터셋 필터링에 대해서도 데이터를 필터링해서 버리는 것 뿐만 아니라 이전에 잘못 버렸던 데이터들을 다시 학습에 사용하는 문제에 대해 언급하고 있는 것이 재미있습니다.

학습 인프라 측면에서는 Zero Bubble Pipeline Parallelism (https://arxiv.org/abs/2401.10241) 을 채택했다는 부분이 흥미롭습니다. 실제로 잘 작동하고 효과가 있는 모양이네요.

#moe #llm 

https://arxiv.org/abs/2405.04434

DeepSeek이 LLM Scaling, 코드, MoE, 수학, Vision Language 등등에 대해 경험을 쌓은 뒤 종합적인 결과를 하나 만들었다는 느낌. 단번에 중국 최상위 수준의 모델에 도달한 동시에 세계적으로도 가장 경쟁력 있는 모델에 등극한 모양새.

지금까지 그랬던 것처럼 테크니컬 리포트가 비교적 상세하다. 기본적으로 21B Activated / 236B Total Parameter, 8.1T 학습한 MoE 모델이다. 그런데 DeepSeek 모델들이 종종 그랬던 것처럼 세팅에 좀 특이한 부분들이 있다.

1. Multi-Head Latent Attention

7B 모델에서 MQA와 GQA에서 성능 손실이 발생했다는 이야기를 한다. 아마도 더 큰 모델에서는 큰 문제가 아닐 수 있을 듯 한데 그냥 추론 시점의 메모리 효율성과 성능을 둘 다 달성할 수 있는 방법을 고안했다.

요약하자면 Attention의 입력 임베딩을 작은 크기로 Projection한 다음 높은 차원으로 다시 Projection을 하는 방법이다. 추론 시에는 작은 크기로 Projection한 Key/Value 캐시만 사용해서 메모리 요구량을 줄인다. 이걸로 MHA보다 더 나은 성능이 나왔다는 이야기를 한다.

아니 성능이 비슷한 것도 아니고 더 나을 이유는 무엇인가? 단서가 있다면 512 차원으로 차원 축소를 하지만 헤드의 수를 임베딩 차원 / 헤드 차원으로 설정하는 대신 임의로 더 많은 수의 헤드를 사용했다는 점에 있을 것이다.

