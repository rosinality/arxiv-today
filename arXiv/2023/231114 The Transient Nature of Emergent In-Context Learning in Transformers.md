https://arxiv.org/abs/2311.08360

The Transient Nature of Emergent In-Context Learning in Transformers (Aaditya K. Singh, Stephanie C.Y. Chan, Ted Moskovitz, Erin Grant, Andrew M. Saxe, Felix Hill)

주어진 맥락을 통해 예측하는 in-context learning과 모델이 학습 과정에서 기억한 것을 통해 예측하는 in-weights learning. omniglot을 사용한 토이 과제에서 학습이 길어지면 in-context learning 능력은 피크를 찍었다가 감소하고 in-weights learning이 점점 더 증가한다는 것이 나타났네요.

왜 in-weight learning이 in-context learning보다 선호될까요? 어쩌면 in-context learning에서 soft attention으로 copy 하는 과정에서 발생하는 에러를 고려했을 때 샘플을 기억해버리는 것이 더 정확할 수 있어서일 수도 있겠습니다. 그러면 애초에 in-context learning이 초반에 더 두드러지게 나타나는 이유는 무엇인가? 그건 알기 어렵네요.

데이터가 크고, 클래스가 많고, 임베딩이 크고, zipf 분포를 따르고, regularization이 걸리면 이 경향이 약화되거나 사라진다는 것으로 나타나서 자연어에서 문제가 되지는 않을 것 같습니다. 다만 in-context learning이 모델 학습 과정에서 임의적으로 나타나는 능력일 수 있다는 사실 자체가 흥미로운 듯 싶네요.

#in_context_learning 