https://arxiv.org/abs/2409.15647

*Looped Transformers for Length Generalization* (Ying Fan, Yilun Du, Kannan Ramchandran, Kangwook Lee)

> Recent work has shown that Transformers trained from scratch can successfully solve various arithmetic and algorithmic tasks, such as adding numbers and computing parity. While these Transformers generalize well on unseen inputs of the same length, they struggle with length generalization, i.e., handling inputs of unseen lengths. In this work, we demonstrate that looped Transformers with an adaptive number of steps significantly improve length generalization. We focus on tasks with a known iterative solution, involving multiple iterations of a RASP-L operation - a length-generalizable operation that can be expressed by a finite-sized Transformer. We train looped Transformers using our proposed learning algorithm and observe that they learn highly length-generalizable solutions for various tasks.

RASP-L이라는 제한된 형태의 프로그램을 실행하도록 Universal Transformer처럼 같은 레이어를 반복 사용하는 모델을 학습. 여기서 Length Generalization이 가능하게 한 방법은 프로그램을 실행하는데 필요한 단계의 수만큼 레이어를 반복 적용했다는 것이네요.

실용적으로 필요한 반복 횟수를 알 수 있는 문제는 별로 없겠지만...Universal Transformer처럼 특정한 구조를 주입하는 것이 일반화 가능한 모델로 이어진다는 사례 중 하나로 생각할 수 있겠군요.

#transformer 