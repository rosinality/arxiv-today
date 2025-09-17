https://arxiv.org/abs/2507.10532

*Reasoning or Memorization? Unreliable Results of Reinforcement Learning Due to Data Contamination* (Mingqi Wu, Zhihao Zhang, Qiaole Dong, Zhiheng Xi, Jun Zhao, Senjie Jin, Xiaoran Fan, Yuhao Zhou, Yanwei Fu, Qin Liu, Songyang Zhang, Qi Zhang)

> The reasoning capabilities of large language models (LLMs) have been a longstanding focus of research. Recent works have further enhanced these capabilities using reinforcement learning (RL), with many new methods claiming significant improvements with minimal or no external supervision. Surprisingly, some studies even suggest that random or incorrect reward signals can enhance reasoning performance. However, these breakthroughs are mostly reported on the Qwen2.5 model family and evaluated on well-known benchmarks such as MATH-500, AMC, and AIME, while failing to achieve similar gains on other models like Llama, which warrants further investigation. Our analysis shows that although Qwen2.5 achieves strong mathematical reasoning performance, its pretraining on large-scale web corpora makes it vulnerable to data contamination in popular benchmarks. As a result, results derived from these benchmarks may be unreliable. To address this, we introduce a generator that produces fully synthetic arithmetic problems of arbitrary length and difficulty, yielding a clean dataset we call RandomCalculation. Using these leakage-free datasets, we show that only accurate reward signals consistently improve performance, while noisy or incorrect signals do not. We advocate for evaluating RL methods on uncontaminated benchmarks and across diverse model families to ensure trustworthy conclusions.

Qwen이 잘못된 Reward로도 추론 학습이 가능한 것은 (https://arxiv.org/abs/2506.10947) 프리트레이닝 데이터셋 오염 때문일 수 있다는 주장. 생성한 데이터셋으로 학습시키면 Reward가 올바른 경우에만 학습이 된다고 하는군요.

<english>
An insist that the reason why it is possible to train Qwen to reason with wrong rewards could be due to dataset contamination. If we train it with synthesized data then it is only possible to train it with correct rewards.
</english>

#rl #reasoning 