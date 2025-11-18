https://arxiv.org/abs/2511.13027

*Scaling Generative Verifiers For Natural Language Mathematical Proof Verification And Selection* (Sadegh Mahdavi, Branislav Kisacanin, Shubham Toshniwal, Wei Du, Ivan Moshkov, George Armstrong, Renjie Liao, Christos Thrampoulidis, Igor Gitman)

> Large language models have achieved remarkable success on final-answer mathematical problems, largely due to the ease of applying reinforcement learning with verifiable rewards. However, the reasoning underlying these solutions is often flawed. Advancing to rigorous proof-based mathematics requires reliable proof verification capabilities. We begin by analyzing multiple evaluation setups and show that focusing on a single benchmark can lead to brittle or misleading conclusions. To address this, we evaluate both proof-based and final-answer reasoning to obtain a more reliable measure of model performance. We then scale two major generative verification methods (GenSelect and LLM-as-a-Judge) to millions of tokens and identify their combination as the most effective framework for solution verification and selection. We further show that the choice of prompt for LLM-as-a-Judge significantly affects the model's performance, but reinforcement learning can reduce this sensitivity. However, despite improving proof-level metrics, reinforcement learning does not enhance final-answer precision, indicating that current models often reward stylistic or procedural correctness rather than mathematical validity. Our results establish practical guidelines for designing and evaluating scalable proof-verification and selection systems.

증명 검증을 위한 Generative Verifier 구축. 그렇지만 별로 성공적이지 않았음. 모델이 표면적인 특징으로 해킹하는 경향이 나타남. 해킹 불가능한 보상을 어떻게 부여할 수 있을지?

Building a generative verifier for proof verification, but it was not very successful - models tend to hack using surface-level features. How can we assign non-hackable reward for this?

#reward-model #rl #reasoning 