https://arxiv.org/abs/2502.14768

*Logic-RL: Unleashing LLM Reasoning with Rule-Based Reinforcement Learning* (Tian Xie, Zitian Gao, Qingnan Ren, Haoming Luo, Yuqian Hong, Bryan Dai, Joey Zhou, Kai Qiu, Zhirong Wu, Chong Luo)

> Inspired by the success of DeepSeek-R1, we explore the potential of rule-based reinforcement learning (RL) in large reasoning models. To analyze reasoning dynamics, we use synthetic logic puzzles as training data due to their controllable complexity and straightforward answer verification. We make some key technical contributions that lead to effective and stable RL training: a system prompt that emphasizes the thinking and answering process, a stringent format reward function that penalizes outputs for taking shortcuts, and a straightforward training recipe that achieves stable convergence. Our 7B model develops advanced reasoning skills-such as reflection, verification, and summarization-that are absent from the logic corpus. Remarkably, after training on just 5K logic problems, it demonstrates generalization abilities to the challenging math benchmarks AIME and AMC.

논리 퍼즐로 추론 RL을 학습시킨 결과가 나왔네요. 데이터는 전형적인 거짓말을 찾는 문제입니다. RL에서 일반화가 두드러진다는 것과 논리 퍼즐에 대해 학습시켰을 때 수학 문제에 대한 성능도 높아진다는 것을 발견했네요.

<english>
The result of doing reasoning RL with logic puzzles appeared. Data is conventional problem of find out liar (Knights and Knaves). They found generalization behavior more apparent on RL and performance on mathematical benchmarks enhances when trained on logic puzzles.
</english>

#reasoning #rl 