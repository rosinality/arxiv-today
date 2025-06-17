https://arxiv.org/abs/2309.16588

Vision Transformers Need Registers (Timothée Darcet, Maxime Oquab, Julien Mairal, Piotr Bojanowski)

DINO (https://arxiv.org/abs/2104.14294) 같은 경우 외의 일반적인 ViT에서 (DINOv2의 경우에도) attention map을 열어보면 이미지 내의 객체에 예쁘게 정렬되어 있는 것이 아니라 군데군데 이미지 내 다른 영역에 튀는 패턴이 나타나는데, 이 문제에 대해 탐색했습니다. 이 튀는 토큰들을 보면 norm이 높고, 로컬한 정보는 없고 글로벌한 정보가 주로 들어 있다고 하네요. 근처 패치들과 비슷해서 중복된 정보가 많은 경우에 이 정보를 무시하고 글로벌한 정보를 처리하기 위해 사용한다는 것을 시사하네요. 글로벌한 정보를 처리하는 것 자체는 유용하지만 dense prediction 케이스를 생각하면 중요한 로컬 정보가 날아간다는 의미이기도 하죠.

그래서 이런 글로벌한 정보 처리를 위해 쓸 수 있는 토큰(레지스터)들을 몇 개 추가해줬습니다. 그랬을 때 attention map에서 발생하던 패턴들이 사라지고, 성능 또한 좀 더 향상되는 군요. Streaming LM과는 좀 다른 원인이긴 하지만 (https://arxiv.org/abs/2309.17453) 모델이 임의로 사용할 수 있는 토큰을 추가한다는 공통적인 아이디어는 흥미롭지 않나 싶습니다. 사실 토큰과 임베딩, 출력이 모두 일대일 대응되어야 할 필요는 없죠.

#vit #transformer

# Links

[[210429 Emerging Properties in Self-Supervised Vision Transformers.md]]
[[230929 Efficient Streaming Language Models with Attention Sinks.md]]