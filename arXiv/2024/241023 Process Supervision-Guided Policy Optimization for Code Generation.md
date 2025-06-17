https://arxiv.org/abs/2410.17621

*Process Supervision-Guided Policy Optimization for Code Generation* (Ning Dai, Zheng Wu, Renjie Zheng, Ziyun Wei, Wenlei Shi, Xing Jin, Guanlin Liu, Chen Dun, Liang Huang, Lin Yan)

> Reinforcement Learning (RL) with unit test feedback has enhanced large language models (LLMs) code generation, but relies on sparse rewards provided only after complete code evaluation, limiting learning efficiency and incremental improvements. When generated code fails all unit tests, no learning signal is received, hindering progress on complex tasks. To address this, we propose a Process Reward Model (PRM) that delivers dense, line-level feedback on code correctness during generation, mimicking human code refinement and providing immediate guidance. We explore various strategies for training PRMs and integrating them into the RL framework, finding that using PRMs both as dense rewards and for value function initialization significantly boosts performance. Our approach increases our in-house LLM's pass rate from 28.2% to 29.8% on LiveCodeBench and from 31.8% to 35.8% on our internal benchmark. Our experimental results highlight the effectiveness of PRMs in enhancing RL-driven code generation, especially for long-horizon scenarios.

코드에 대한 Process Reward Model. 코드 중간을 자른 다음 나머지 부분을 생성시키고 이 생성 결과 중에서 유닛 테스트를 통과하는 결과가 나오는가로 이전 부분의 코드에 대한 보상을 부여하는 방법이네요.

다만 (수학도 그렇지만) 각 코드 Prefix에 대한 보상이라는 것 자체가 코드만으로는 부여하기 좀 어려운 대상이라는 생각도 드는군요. 코드의 각 라인의 가치는 문제를 해결하기 위한 전략과 계획에 부합하는가 아닌가에 있겠죠. 물론 이런 전략과 계획에 대해서도 평가를 할 수 있겠고, 각 코드 라인의 정확성도 평가할 수 있겠지만요.

<english>
Process reward model for the code. Split middle position of the code, and generate rest of it, and among generated samples, and assings reward by checking whether there are samples that could pass the unit tests.

But (similar to math) I think it may be hard to assign rewards for each code prefixes. Value of each line of codes are lie in whether it is compatible to strategies and plans to solve the problem. Of course you can evaluate these strategies and plans, and also accuracy of the each code lines.
</english>

#reward-model #code 