https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/blob/main/ORZ_paper.pdf

*Open-Reasoner-Zero: An Open Source Approach to Scaling Up Reinforcement Learning on the Base Model* (Jingcheng Hu, Yinmin Zhang, Qi Han, Daxin Jiang, Xiangyu Zhang, Heung-Yeung Shum)

> We introduce Open-Reasoner-Zero, the first open source implementation of large-scale reasoning-oriented RL training focusing on scalability, simplicity and accessibility. Through extensive experiments, we demonstrate that a minimalist approach, vanilla PPO with GAE (𝜆 = 1, 𝛾 = 1) and straightforward rule-based reward function, without any KL regularization, is sufficient to scale up both response length and benchmark performance on reasoning tasks, similar to the phenomenon observed in DeepSeek-R1-Zero. Notably, our implementation outperforms DeepSeek-R1-Zero-Qwen-32B on the GPQA Diamond benchmark, while only requiring 1/30 of the training steps. In the spirit of open source, we release our source code, parameter settings, training data, and model weights.

StepFun에서 RL CoT 실험 결과를 공개했군요. KL Penalty 없는 바닐라 PPO 사용.

<english>
StepFun released experiment results on RL CoT. They used vanilla PPO without KL penalty.
</english>

#reasoning #rl 