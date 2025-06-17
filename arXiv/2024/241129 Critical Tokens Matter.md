https://arxiv.org/abs/2411.19943

*Critical Tokens Matter: Token-Level Contrastive Estimation Enhence LLM's Reasoning Capability* (Zicheng Lin, Tian Liang, Jiahao Xu, Xing Wang, Ruilin Luo, Chufan Shi, Siheng Li, Yujiu Yang, Zhaopeng Tu)

> Large Language Models (LLMs) have exhibited remarkable performance on reasoning tasks. They utilize autoregressive token generation to construct reasoning trajectories, enabling the development of a coherent chain of thought. In this work, we explore the impact of individual tokens on the final outcomes of reasoning tasks. We identify the existence of ``critical tokens'' that lead to incorrect reasoning trajectories in LLMs. Specifically, we find that LLMs tend to produce positive outcomes when forced to decode other tokens instead of critical tokens. Motivated by this observation, we propose a novel approach - cDPO - designed to automatically recognize and conduct token-level rewards for the critical tokens during the alignment process. Specifically, we develop a contrastive estimation approach to automatically identify critical tokens. It is achieved by comparing the generation likelihood of positive and negative models. To achieve this, we separately fine-tune the positive and negative models on various reasoning trajectories, consequently, they are capable of identifying identify critical tokens within incorrect trajectories that contribute to erroneous outcomes. Moreover, to further align the model with the critical token information during the alignment process, we extend the conventional DPO algorithms to token-level DPO and utilize the differential likelihood from the aforementioned positive and negative model as important weight for token-level DPO learning.Experimental results on GSM8K and MATH500 benchmarks with two-widely used models Llama-3 (8B and 70B) and deepseek-math (7B) demonstrate the effectiveness of the propsoed approach cDPO.

LLM의 추론 과정에서 오답을 유도하는 결정적인 토큰이 있다는 발견. 첫 토큰의 중요성도 생각나는 결과네요. (https://arxiv.org/abs/2402.10200) 이 결정적인 토큰을 찾아 억제하는 것으로 추론 성능을 높일 수 있다는 아이디어입니다.

<english>
Observation on the existence of critical tokens that induces incorrect answers while reasoning proces of LLMs. It reminds me of importance of first token. (https://arxiv.org/abs/2402.10200) So we can enhance reasoning performance by find out these critical tokens and suppress it.
</english>

#reasoning

# Links

[[240215 Chain-of-Thought Reasoning Without Prompting.md]]