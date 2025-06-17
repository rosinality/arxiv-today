https://arxiv.org/abs/2501.11651

*Advancing Language Model Reasoning through Reinforcement Learning and Inference Scaling* (Zhenyu Hou, Xin Lv, Rui Lu, Jiajie Zhang, Yujiang Li, Zijun Yao, Juanzi Li, Jie Tang, Yuxiao Dong)

> Large language models (LLMs) have demonstrated remarkable capabilities in complex reasoning tasks. However, existing approaches mainly rely on imitation learning and struggle to achieve effective test-time scaling. While reinforcement learning (RL) holds promise for enabling self-exploration and learning from feedback, recent attempts yield only modest improvements in complex reasoning. In this paper, we present T1 to scale RL by encouraging exploration and understand inference scaling. We first initialize the LLM using synthesized chain-of-thought data that integrates trial-and-error and self-verification. To scale RL training, we promote increased sampling diversity through oversampling. We further employ an entropy bonus as an auxiliary loss, alongside a dynamic anchor for regularization to facilitate reward optimization. We demonstrate that T1 with open LLMs as its base exhibits inference scaling behavior and achieves superior performance on challenging math reasoning benchmarks. For example, T1 with Qwen2.5-32B as the base model outperforms the recent Qwen QwQ-32B-Preview model on MATH500, AIME2024, and Omni-math-500. More importantly, we present a simple strategy to examine inference scaling, where increased inference budgets directly lead to T1's better performance without any additional verification. We will open-source the T1 models and the data used to train them at https://github.com/THUDM/T1.

정답 기반 RL CoT. 높은 Temperature와 엔트로피 보너스를 사용해서 더 다양한 샘플을 많이 생성하는 것이 효과적이라는 결론. R1이나 Kimi 1.5도 방법상 여러 샘플을 사용하긴 하죠.

<english>
RL CoT based on correctness. The conclusion is it is better to use more diverse samples using high temperature and entropy bonus. Actually R1 and Kimi 1.5 uses multiple samples per prompt due to their methods.
</english>

#rl #reasoning 