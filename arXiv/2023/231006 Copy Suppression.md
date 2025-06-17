https://arxiv.org/abs/2310.04625

Copy Suppression: Comprehensively Understanding an Attention Head (Callum McDougall, Arthur Conmy, Cody Rushing, Thomas McGrath, Neel Nanda)

GPT-2 Small에서 Negative Heads라는 Attention Head를 발견했습니다. 트랜스포머의 초기 레이어에서는 이전에 나온 토큰을 가져와서 바로 출력으로 복붙하는 경향이 있는데, 이 Negative Heads는 이러한 복붙을 감지해서 복사한 토큰의 확률을 낮추는 방향으로 작동한다고 하네요. 토큰 검출 뉴런이 검출한 토큰의 확률을 억제한다는 결과가 있었는데 (https://arxiv.org/abs/2309.04827) 결합해서 생각해볼 수 있지 않을까 싶네요.

#transformer #lm

# Links

[[230909 Neurons in Large Language Models.md]]