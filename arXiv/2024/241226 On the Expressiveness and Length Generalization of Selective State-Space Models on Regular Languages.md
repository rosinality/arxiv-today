https://arxiv.org/abs/2412.19350

*On the Expressiveness and Length Generalization of Selective State-Space Models on Regular Languages* (Aleksandar Terzić, Michael Hersche, Giacomo Camposampiero, Thomas Hofmann, Abu Sebastian, Abbas Rahimi)

> Selective state-space models (SSMs) are an emerging alternative to the Transformer, offering the unique advantage of parallel training and sequential inference. Although these models have shown promising performance on a variety of tasks, their formal expressiveness and length generalization properties remain underexplored. In this work, we provide insight into the workings of selective SSMs by analyzing their expressiveness and length generalization performance on regular language tasks, i.e., finite-state automaton (FSA) emulation. We address certain limitations of modern SSM-based architectures by introducing the Selective Dense State-Space Model (SD-SSM), the first selective SSM that exhibits perfect length generalization on a set of various regular language tasks using a single layer. It utilizes a dictionary of dense transition matrices, a softmax selection mechanism that creates a convex combination of dictionary matrices at each time step, and a readout consisting of layer normalization followed by a linear map. We then proceed to evaluate variants of diagonal selective SSMs by considering their empirical performance on commutative and non-commutative automata. We explain the experimental results with theoretical considerations. Our code is available at https://github.com/IBM/selective-dense-state-space-model.

State Space Model의 표현력에 대한 연구. (https://arxiv.org/abs/2404.08819, https://arxiv.org/abs/2405.17394) 여기에서는 각 스텝의 Transition 행렬을 스텝마다 다르게 만드는 방법으로 접근했네요.

최근에 RWKV-7도 비슷한 문제를 이야기하던데 RWKV-7은 Test Time Train을 사용했군요. (https://github.com/BlinkDL/RWKV-LM)

<english>
The study on representational capacity of state space model (https://arxiv.org/abs/2404.08819, https://arxiv.org/abs/2405.17394). This study approached this limited capacity problem by using distinct transition matrices for each steps.

Recently RWKV-7 mentioned similar problems, and it used test time train (https://github.com/BlinkDL/RWKV-LM).
</english>

#state-space-model

# Links

[[240412 The Illusion of State in State-Space Models.md]]