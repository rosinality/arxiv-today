https://arxiv.org/abs/2311.10768

Memory Augmented Language Models through Mixture of Word Experts (Cicero Nogueira dos Santos, James Lee-Thorp, Isaac Noble, Chung-Ching Chang, David Uthus)

단어 기반 routing을 하는 MoE. 여기서 단어는 입력 토큰 그대로가 아니라 위키피디아를 사용해 구축된, 더 많은 vocabulary를 갖는 단어입니다. 그리고 이 단어에 expert를 분배합니다. 즉 하나의 단어를 구성하는 여러 subword에 대해 하나의 expert가 부여되게 되죠.

그리고 expert의 크기를 줄이는 대신 8K, 32K 까지 숫자를 늘렸습니다. 이를 통해 각 expert가 각 단어에 관련된 지식를 저장하는 일종의 외부 메모리로 기능할 수 있다고 기대하고 있네요.

새로운 토크나이저를 사용한다는 것이 좀 신경쓰이긴 하지만 routing 문제를 해결해서 expert의 수를 훨씬 더 늘리고 sparse activation을 한다면 retrieval 기반 lm처럼 지식을 모델에서 분리하는 괜찮은 방법이지 않나 싶기는 하네요.

#moe 