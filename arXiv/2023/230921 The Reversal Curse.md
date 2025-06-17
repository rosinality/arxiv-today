https://arxiv.org/abs/2309.12288

The Reversal Curse: LLMs trained on "A is B" fail to learn "B is A" (Lukas Berglund, Meg Tong, Max Kaufmann, Mikita Balesni, Asa Cooper Stickland, Tomasz Korbak, Owain Evans)

LM이 A는 B다라는 텍스트로 학습되었을 때 B는 A라는 일반화가 가능한지에 대한 테스트. 여러 조건에서 해봤지만 안 되더라는 결론입니다. 원인으로 추측한 이유가 재미있네요. A는 B다라는 텍스트로 학습을 하면 A 임베딩에 B의 정보가 들어가게 될 텐데, 대칭적이라면 B에도 A에 대한 정보가 들어가야겠지만 그렇게 되리라는 보장이 없죠.

대칭성의 문제가 되는 것 같은데, 적절한 대칭성이 이런 문제에 큰 도움이 될 수 있겠죠. 그렇지만 자연어에 대해서 우리가 어떤 적절한 대칭성을 모델에 주입할 수 있을까요?

#generalization #lm 