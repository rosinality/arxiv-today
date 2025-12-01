https://github.com/deepseek-ai/DeepSeek-Math-V2/blob/main/DeepSeekMath_V2.pdf

*DeepSeekMath-V2: Towards Self-Verifiable Mathematical Reasoning* (Zhihong Shao, Yuxiang Luo, Chengda Lu, Z.Z. Ren, Jiewen Hu, Tian Ye, Zhibin Gou, Shirong Ma, Xiaokang Zhang)

> Large language models have made significant progress in mathematical reasoning, which serves as an important testbed for AI and could impact scientific research if further advanced. By scaling reasoning with reinforcement learning that rewards correct final answers, LLMs have improved from poor performance to saturating quantitative reasoning competitions like AIME and HMMT in one year. However, this approach faces fundamental limitations. Pursuing higher final answer accuracy doesn’t address a key issue: correct answers don’t guarantee correct reasoning. Moreover, many mathematical tasks like theorem proving require rigorous step-by-step derivation rather than numerical answers, making final answer rewards inapplicable. To push the limits of deep reasoning, we believe it is necessary to verify the comprehensiveness and rigor of mathematical reasoning. Self-verification is particularly important for scaling test- time compute, especially for open problems without known solutions. Towards self-verifiable mathematical reasoning, we investigate how to train an accurate and faithful LLM-based verifier for theorem proving. We then train a proof generator using the verifier as the reward model, and incentivize the generator to identify and resolve as many issues as possible in their own proofs before finalizing them. To maintain the generation-verification gap as the generator becomes stronger, we propose to scale verification compute to automatically label new hard- to-verify proofs, creating training data to further improve the verifier. Our resulting model, DeepSeekMath-V2, demonstrates strong theorem-proving capabilities, achieving gold-level scores on IMO 2025 and CMO 2024 and a near-perfect 118/120 on Putnam 2024 with scaled test- time compute. While much work remains, these results suggest that self-verifiable mathematical reasoning is a feasible research direction that may help develop more capable mathematical AI systems.

DeepSeek의 증명 모델. 증명과 같이 단순한 검증 방법이 존재하지 않는 문제에 대해서 모델을 어떻게 학습시킬 수 있는지를 보여주는 결과. 메타-검증이 핵심 아이디어.

1. 검증 모델을 학습. 검증 모델은 검증의 정답 여부를 사용해 학습시킬 수 있음. 그러나 이것만으로는 검증 모델이 실제 문제를 포착하지 못하고 할루시네이션을 발생시키는 것을 막을 수 없음. 그래서 여기서는 메타 검증 모델을 사용해 검증 모델이 찾아낸 문제를 검증하도록 함.

2. 증명 모델이 검증과 메타 검증 결과를 보상으로 사용해서 자기 검증을 하도록 함.

3. 증명 모델과 검증 모델 사이의 일종의 Self-Play. 그렇지만 새로운 증명에 대한 레이블을 만들어야 함. 이에 대해서 AI의 도움을 받아 어노테이션을 진행.

일단 N번 검증을 진행하고 검증 과정에서 파악된 문제에 대해서 메타-검증을 M번 수행. 여기서 k개의 정당한 문제가 발견되었다면 증명은 오류로 처리. 아무런 문제가 발견되지 않았다면 정답으로 처리함. 완화된 Pessimistic Scoring이라고 생각할 수 있음.

This shows how we can train a model on problems like proving for which a simple verification method does not exist. Meta-verification is the central idea of this.

1. Train verifiers. We can train verifiers using correctness rewards - but this cannot ensure that the verifier points out a real issue, not hallucinations. Thus this paper uses meta verifiers that verify the issues that verifiers found.

2. Train provers to do self-verification using verification and meta-verification rewards.

3. A kind of self-play between prover and verifier. But we need to create labels for new proofs. This is done by AI-assisted manual annotation.

First verification is done N times, and for issues found in verification, meta-verification is done M times. If they find k legitimate issues then it is incorrect. If no issues are found it is considered correct. A relaxed pessimistic scoring.

#rl #reasoning #math #reward-model 