https://arxiv.org/abs/2509.22611

*Quantile Advantage Estimation for Entropy-Safe Reasoning* (Junkang Wu, Kexin Huang, Jiancan Wu, An Zhang, Xiang Wang, Xiangnan He)

> Reinforcement Learning with Verifiable Rewards (RLVR) strengthens LLM reasoning, but training often oscillates between {entropy collapse} and {entropy explosion}. We trace both hazards to the mean baseline used in value-free RL (e.g., GRPO and DAPO), which improperly penalizes negative-advantage samples under reward outliers. We propose {Quantile Advantage Estimation} (QAE), replacing the mean with a group-wise K-quantile baseline. QAE induces a response-level, two-regime gate: on hard queries (p <= 1 - K) it reinforces rare successes, while on easy queries (p > 1 - K) it targets remaining failures. Under first-order softmax updates, we prove {two-sided entropy safety}, giving lower and upper bounds on one-step entropy change that curb explosion and prevent collapse. Empirically, this minimal modification stabilizes entropy, sparsifies credit assignment (with tuned K, roughly 80% of responses receive zero advantage), and yields sustained pass@1 gains on Qwen3-8B/14B-Base across AIME 2024/2025 and AMC 2023. These results identify {baseline design} -- rather than token-level heuristics -- as the primary mechanism for scaling RLVR.

DAPO가 Negative Advantage에 의한 엔트로피 폭발 문제를 겪는다는 분석. GRPO의 평균을 통한 Noramlization을 Quantile을 사용한 베이스라인으로 교체. 엔트로피 통제 문제는 탐험의 여지가 많은 영역이라고 생각.

DAPO suffers from entropy explosion problems driven by negative advantages. The authors replaced the mean shift in GRPO with a quantile-based baseline. I think this entropy control problem is a rich source of exploration.

#rl #reasoning 