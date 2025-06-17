https://arxiv.org/abs/2504.21801

*DeepSeek-Prover-V2: Advancing Formal Mathematical Reasoning via Reinforcement Learning for Subgoal Decomposition* (Z.Z. Ren, Zhihong Shao, Junxiao Song, Huajian Xin, Haocheng Wang, Wanjia Zhao, Liyue Zhang, Zhe Fu, Qihao Zhu, Dejian Yang, Z.F. Wu, Zhibin Gou, Shirong Ma, Hongxuan Tang, Yuxuan Liu, Wenjun Gao, Daya Guo, Chong Ruan)

> We introduce DeepSeek-Prover-V2, an open-source large language model designed for formal theorem proving in Lean 4, with initialization data collected through a recursive theorem proving pipeline powered by DeepSeek-V3. The cold-start training procedure begins by prompting DeepSeek-V3 to decompose complex problems into a series of subgoals. The proofs of resolved subgoals are synthesized into a chain-of-thought process, combined with DeepSeek-V3's step-by-step reasoning, to create an initial cold start for reinforcement learning. This process enables us to integrate both informal and formal mathematical reasoning into a unified model. The resulting model, DeepSeek-Prover-V2-671B, achieves state-of-the-art performance in neural theorem proving, reaching 88.9% pass ratio on the MiniF2F-test and solving 49 out of 658 problems from PutnamBench. In addition to standard benchmarks, we introduce ProverBench, a collection of 325 formalized problems, to enrich our evaluation, including 15 selected problems from the recent AIME competitions (years 24-25). Further evaluation on these 15 AIME problems shows that the model successfully solves 6 of them. In comparison, DeepSeek-V3 solves 8 of these problems using majority voting, highlighting that the gap between formal and informal mathematical reasoning in large language models is substantially narrowing.

DeepSeek의 증명 추론 모델. 정리를 세부 목표로 쪼갠 다음 각 목표를 작은 모델로 증명해서 전체 증명을 완성하는 방식으로 데이터를 구축했습니다. 이를 기반으로 추론 모드와 비추론 모드를 학습시켰네요. Lean 4를 사용한 증명 연구를 했던 것이 계속 도움이 되는군요.

<english>
DeepSeek's reasoning proving model. Constructs the data by decomposing a theorem into subgoals and complete overall theorem through prove each goals using smaller models. Based on this they trained a model with reasoning and non-reasoning mode. I think previous reasearch they did on proof using Lean 4 is continuously help for them.
</english>

#math #reasoning #rl 