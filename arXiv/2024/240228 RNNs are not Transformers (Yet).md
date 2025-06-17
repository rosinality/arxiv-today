https://arxiv.org/abs/2402.18510

*RNNs are not Transformers (Yet): The Key Bottleneck on In-context Retrieval* (Kaiyue Wen, Xingyu Dang, Kaifeng Lyu)

> This paper investigates the gap in representation powers of Recurrent Neural Networks (RNNs) and Transformers in the context of solving algorithmic problems. We focus on understanding whether RNNs, known for their memory efficiency in handling long sequences, can match the performance of Transformers, particularly when enhanced with Chain-of-Thought (CoT) prompting. Our theoretical analysis reveals that CoT improves RNNs but is insufficient to close the gap with Transformers. A key bottleneck lies in the inability of RNNs to perfectly retrieve information from the context, even with CoT: for several tasks that explicitly or implicitly require this capability, such as associative recall and determining if a graph is a tree, we prove that RNNs are not expressive enough to solve the tasks while Transformers can solve them with ease. Conversely, we prove that adopting techniques to enhance the in-context retrieval capability of RNNs, including Retrieval-Augmented Generation (RAG) and adding a single Transformer layer, can elevate RNNs to be capable of solving all polynomial-time solvable problems with CoT, hence closing the representation gap with Transformers.

RNN의 표현력 한계에 대한 연구. 결국 Context 내의 정보에 대한 Retrieval의 한계가 문제가 됩니다. 그리고 그 한계를 해소할 수 있는 것은 Retrieval 메커니즘의 결합이고 그에 대해 가장 간단한 방법은 (명시적으로 할 수도 있겠지만) 트랜스포머 레이어를 추가하는 것이죠.

여러모로 SSM이 쓰이더라도 트랜스포머와의 하이브리드가 맞는 방향이 아닐까 싶습니다. Based 같이 Linear Attention 내에서 해결하려는 시도도 있긴 합니다만 아무래도 좀 더 어려운 경로가 될 것 같네요.

#transformer #rnn #state-space-model