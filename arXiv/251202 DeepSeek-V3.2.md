https://huggingface.co/deepseek-ai/DeepSeek-V3.2/blob/main/assets/paper.pdf

*DeepSeek-V3.2: Pushing the Frontier of Open Large Language Models* (DeepSeek-AI)

> We introduce DeepSeek-V3.2, a model that harmonizes high computational efficiency with superior reasoning and agent performance. The key technical breakthroughs of DeepSeek-V3.2 are as follows: (1) DeepSeek Sparse Attention (DSA): We introduce DSA, an efficient attention mechanism that substantially reduces computational complexity while preserving model performance in long-context scenarios. (2) Scalable Reinforcement Learning Framework: By implementing a robust reinforcement learning protocol and scaling post-training compute, DeepSeek-V3.2 performs comparably to GPT-5. Notably, our high-compute variant, DeepSeek-V3.2-Speciale, surpasses GPT-5 and exhibits reasoning proficiency on par with Gemini-3.0-Pro, achieving gold-medal performance in both the 2025 International Mathematical Olympiad (IMO) and the International Olympiad in Informatics (IOI). (3) Large-Scale Agentic Task Synthesis Pipeline: To integrate reasoning into tool-use scenarios, we developed a novel synthesis pipeline that systematically generates training data at scale. This methodology facilitates scalable agentic post-training, yielding substantial improvements in generalization and instruction-following robustness within complex, interactive environments.

DeepSeek-V3.2(-Speciale) 테크니컬 리포트. DSA와 함께 GRPO 안정화 테크닉 적용. (Unbiased KL 페널티, Loss 마스킹, 라우팅과 샘플링 리플레이). 그리고 합성 데이터베이스를 사용한 합성 에이전트 궤적. Length 페널티를 줄여 Speciale 버전을 구축.

DeepSeek-V3.2(-Speciale) technical report. DSA and GRPO stabilization techniques (unbiased KL penalty, loss masking, routing and sampling replay). And synthetic agentic trajectory using a synthetic database. They made the Speciale version using reduced length penalty.

#rl #reasoning #agent #synthetic-data 