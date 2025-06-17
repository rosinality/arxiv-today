https://research.character.ai/optimizing-inference/

*Optimizing AI Inference at Character.AI* (Character.AI)

Character.AI의 추론 최적화를 위한 아키텍처 변형.

1. GQA 대신 MQA
2. Local Attention 5 + Global Attention 1 레이어 조합
3. 레이어 간 KV 캐시 공유.
4. Radix Attention과 비슷하게 KV 캐시를 트리로 구성해 여러 턴 사이에서도 KV 캐시를 공유
5. Weight, Activation, KV Cache에 대한 Int8 Quantization. 놀랍게도 PTQ가 아니라 Int8 학습을 했다고 합니다.

모델 성능을 위한 레시피 뿐만 아니라 추론을 위한 최적화 측면에서도 선두 기업들과의 차이가 크다는 이야기가 있었는데 그것이 좀 드러난 것 같네요. 레이어 간 캐시 공유 같은 것은 최근에야 논문으로 나오고 있는 방법인데 이미 사용하고 있었군요. Int8 학습 같은 것은 거의 알려지지 않았죠.

#transformer #efficiency 