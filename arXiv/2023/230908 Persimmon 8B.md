https://www.adept.ai/blog/persimmon-8b

8B 모델이 하나 나왔군요. 개인적으로 재미있는 부분들.

1. Squared ReLU (!) Primer (https://arxiv.org/abs/2109.08668) 가 여기에서 등장...
2. QK LayerNorm 그러고 보니 ViT-22B (https://arxiv.org/abs/2302.05442) 에서 언급됐던 QK LayerNorm 논문은 아직 안 나왔네요.
3. 시작부터 16K Context Length에서 학습
4. Vocabulary는 262K. 70K는 비워놓음.
5. FasterTransformer에서 Attention 커널을 뜯어와서 CUDA Graph와 조합하는 방식으로 파이토치로 추론하는 코드를 제공. FasterTransformer Attention이 FlashAttention보다 추론 시점에 나은가 보네요.