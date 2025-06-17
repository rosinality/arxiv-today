https://arxiv.org/abs/2310.08461

DistillSpec: Improving Speculative Decoding via Knowledge Distillation (Yongchao Zhou, Kaifeng Lyu, Ankit Singh Rawat, Aditya Krishna Menon, Afshin Rostamizadeh, Sanjiv Kumar, Jean-François Kagy, Rishabh Agarwal)

Speculative Decoding이 효율적이려면 Drafter 모델과 Verifier 모델이 잘 정렬되어 있어서 채택율(Acceptance  rate)이 높은 것이 효과적이겠죠. 채택율을 높이기 위해 Drafter로 생성한 샘플에 대해 distill 한다는 아이디어입니다. 최근에 흡사한 아이디어가 나왔었죠. (https://arxiv.org/abs/2310.07177)

파인튜닝 까지 거치는 과정들을 고려하면 Drafter를 잘 구성하는 것이 까다롭겠다는 생각을 했었는데 그 문제에 대응할 수 있는 도구가 주어졌다는 느낌이네요.

#efficiency #distillation

# Links

[[230202 Accelerating Large Language Model Decoding with Speculative Sampling]]