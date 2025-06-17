https://arxiv.org/abs/2311.08401

Fine-tuning Language Models for Factuality (Katherine Tian, Eric Mitchell, Huaxiu Yao, Christopher D. Manning, Chelsea Finn)

사실과 관련된 할루시네이션을 억제하기. 모델의 생성 결과를 쪼개서 주장들을 추출하고, 이 추출한 주장을 레퍼런스와 결합해서 사실인지 판단하거나 레퍼런스가 없다면 모델의 uncertainty로 평가한 방법입니다. 그리고 이렇게 구축한 사실에 대한 선호를 사용해 DPO를 했네요.

사실과 관련된 피드백으로 할루시네이션을 감소시킬 수 있다는 사례나 결과가 공개된 것 많지 않은 상황에서 그 자체만으로도 흥미로운 결과가 아닐까 싶네요.

#hallucination #alignment 