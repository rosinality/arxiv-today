https://discuss.pytorch.org/t/distributed-w-torchtitan-introducing-async-tensor-parallelism-in-pytorch/209487

*Introducing Async Tensor Parallelism in PyTorch* (Yifu Wang, Horace He, Less Wright, Luca Wehrstedt, Tianyu Liu, Wanchao Liang)

PyTorch에 Async Tensor Parallel 구현이 들어왔군요. 이 방법을 적용한 대표적인 사례가 ViT-22B죠. (https://arxiv.org/abs/2302.05442)

이런 방법의 핵심은 연산과 통신을 중첩하는 것인데 그냥은 구현이 쉽지 않았다고 하는군요. SymmetricMemory라는 추상화 위에 구현되어 있는데 참조해보면 재미있을 것 같습니다.

#parallelism #efficiency 