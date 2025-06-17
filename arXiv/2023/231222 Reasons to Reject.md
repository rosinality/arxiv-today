https://arxiv.org/abs/2312.14591

Reasons to Reject? Aligning Language Models with Judgments (Weiwen Xu, Deng Cai, Zhisong Zhang, Wai Lam, Shuming Shi)

텍스트 Critic (Judgment)로 피드백을 주는 방법. Instruction (x), Response (y), Judgment (j)의 Triplet에서 x, y와 x, y, j가 Align된 경우 (Align-P), 즉 좋은 y를 생성한 경우, x, y, j는 Align 되어 있으나 x, y가 Align 되지 않은 경우, 즉 좋은 y를 생성하지 못한 경우 (Align-N), 그리고 좋은 y를 생성하지 못한 경우에서 j를 Negative가 아니라 임의의 Postive 피드백으로 교환한 경우를 생각합니다 (Misalign).

Align-N은 x, y, j가 Align 되어 있기에 Misalign 보다 확률이 높은 토큰들이 존재하고 이 확률이 높은 토큰들에 Unlikelihood Loss를 줍니다. 그렇지 않은 토큰들과 Align-P, 그리고 Align-N + Judgment에 대해서는 MLE 학습을 하네요.

텍스트 피드백을 사용하는 방법들에 대한 연구들이 종종 나왔었는데 꽤 재미있는 접근이지 않은가 싶습니다. Judgment와 Align 되어 있으니 확률이 높아진다라는 가정에 의존하지만요.

#feedback 