https://arxiv.org/abs/2507.07562

*The Synergy Dilemma of Long-CoT SFT and RL: Investigating Post-Training Techniques for Reasoning VLMs* (Jierun Chen, Tiezheng Yu, Haoli Bai, Lewei Yao, Jiannan Wu, Kaican Li, Fei Mi, Chaofan Tao, Lei Zhu, Manyi Zhang, Xiaohui Li, Lu Hou, Lifeng Shang, Qun Liu)

> Large vision-language models (VLMs) increasingly adopt post-training techniques such as long chain-of-thought (CoT) supervised fine-tuning (SFT) and reinforcement learning (RL) to elicit sophisticated reasoning. While these methods exhibit synergy in language-only models, their joint effectiveness in VLMs remains uncertain. We present a systematic investigation into the distinct roles and interplay of long-CoT SFT and RL across multiple multimodal reasoning benchmarks. We find that SFT improves performance on difficult questions by in-depth, structured reasoning, but introduces verbosity and degrades performance on simpler ones. In contrast, RL promotes generalization and brevity, yielding consistent improvements across all difficulty levels, though the improvements on the hardest questions are less prominent compared to SFT. Surprisingly, combining them through two-staged, interleaved, or progressive training strategies, as well as data mixing and model merging, all fails to produce additive benefits, instead leading to trade-offs in accuracy, reasoning style, and response length. This ``synergy dilemma'' highlights the need for more seamless and adaptive approaches to unlock the full potential of combined post-training techniques for reasoning VLMs.

추론 SFT와 RL의 비교. SFT가 고난이도 문제에 대한 향상이 크고 RL은 성능이 고르게 올라간다고. 둘을 섞으면 보완이 아니라 중간 지점으로 간다고 하네요. RL로 고난이도 문제에 대한 성능을 높이는 것을 생각하는 것이 좋은 방향일지도.

<english>
A comparison on reasoning SFT and RL. SFT enhances more for difficult problems, while RL improves the performance rather consistently. If we mix it then it falls under middle points. Maybe finding the way how to improve on difficult problems with RL would be better direction.
</english>

#rl #reasoning 