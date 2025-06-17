https://arxiv.org/abs/2312.02179

Training Chain-of-Thought via Latent-Variable Inference (Du Phan, Matthew D. Hoffman, David Dohan, Sholto Douglas, Tuan Anh Le, Aaron Parisi, Pavel Sountsov, Charles Sutton, Sharad Vikram, Rif A. Saurous)

Chain-of-Thought 튜닝에 필요한 rationale을 생성할 수 있는가? 하는 연구. rationale을 latent z라고 하고, 프롬프트 x와 정답 y에 대해 p(z | x, y)로 rationale을 생성합니다. privileged information을 사용하는 것이라고 볼 수도 있겠네요. 그 다음 p(z | x)로 rationale들을 생성해가면서 p(y | x, z)로 rationale을 사용해서 답이 나왔는지를 체크하고 맞으면 rationale을 교체합니다.

조금 다른 이야기이긴 한데 모델의 생성 결과를 평가할 수 있다면 모델을 개선할 수 있다는 RL스러운 생각이 들긴 하네요. 그래서 수학 같은 문제에 대해 formal verification으로 뭔가를 할 수 있지 않을까 하는 이야기가 나오는 거겠죠.

#prompt #synthetic-data