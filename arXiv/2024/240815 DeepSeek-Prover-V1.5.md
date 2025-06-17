https://arxiv.org/abs/2408.08152

*DeepSeek-Prover-V1.5: Harnessing Proof Assistant Feedback for Reinforcement Learning and Monte-Carlo Tree Search* (Huajian Xin, Z.Z. Ren, Junxiao Song, Zhihong Shao, Wanjia Zhao, Haocheng Wang, Bo Liu, Liyue Zhang, Xuan Lu, Qiushi Du, Wenjun Gao, Qihao Zhu, Dejian Yang, Zhibin Gou, Z.F. Wu, Fuli Luo, Chong Ruan)

> We introduce DeepSeek-Prover-V1.5, an open-source language model designed for theorem proving in Lean 4, which enhances DeepSeek-Prover-V1 by optimizing both training and inference processes. Pre-trained on DeepSeekMath-Base with specialization in formal mathematical languages, the model undergoes supervised fine-tuning using an enhanced formal theorem proving dataset derived from DeepSeek-Prover-V1. Further refinement is achieved through reinforcement learning from proof assistant feedback (RLPAF). Beyond the single-pass whole-proof generation approach of DeepSeek-Prover-V1, we propose RMaxTS, a variant of Monte-Carlo tree search that employs an intrinsic-reward-driven exploration strategy to generate diverse proof paths. DeepSeek-Prover-V1.5 demonstrates significant improvements over DeepSeek-Prover-V1, achieving new state-of-the-art results on the test set of the high school level miniF2F benchmark ($63.5\%$) and the undergraduate level ProofNet benchmark ($25.3\%$).

DeepSeek Prover의 후속 모델. (https://arxiv.org/abs/2405.14333) Proof Assistant 데이터들에 대해 Further Pretraining 한 다음 Lean 4에 대해 SFT. 여기에서 Lean-STaR 식으로 Lean 코드 전에 자연어 Chain of Thought를 달아주는 작업을 진행하고 (https://arxiv.org/abs/2407.10040) Tactic의 상태를 예측하도록 하는 부분도 추가했습니다.

그 다음으로 GRPO와 Proof Assistant의 Verification을 사용한 RL을 수행했네요. 그리고 그 위에 Intrinsic Reward를 사용한 MCTS. 굉장한 프로젝트네요. DeepSeek이 늘 그랬듯.

#math #search 