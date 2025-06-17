https://github.com/ByteDance-Seed/Seed-Coder/blob/master/Seed-Coder.pdf

*Seed-Coder: Let the Code Model Curate Data for Itself* (ByteDance Seed)

> Code data in large language model (LLM) pretraining is recognized crucial not only for code-related tasks but also for enhancing general intelligence of LLMs. Current open-source LLMs often heavily rely on human effort to produce their code pretraining data, such as employing hand-crafted filtering rules tailored to individual programming languages, or using human-annotated data to train quality filters. However, these approaches are inherently limited in scalability, prone to subjective biases, and costly to extend and maintain across diverse programming languages. To address these challenges, we introduce Seed-Coder, a series of open-source LLMs comprising base, instruct and reasoning models of 8B size, minimizing human involvement in data construction. Our code pretraining data is produced by a model-centric data pipeline, which predominantly leverages LLMs for scoring and filtering code data. The instruct model is further trained via supervised fine- \tuning and preference optimization, and the reasoning model leverages Long-Chain-of-Thought (LongCoT) reinforcement learning to improve multi-step code reasoning. Seed-Coder achieves state-of-the-art results among open-source models of similar size and even surpasses some much larger models, demonstrating superior performance in code generation, code completion, code editing, code reasoning, and software engineering tasks.

바이트댄스의 코드 모델. 휴리스틱 필터링 대신 LLM 필터링에 집중한다는 아이디어 (https://arxiv.org/abs/2412.02595). 준비된 모델이 없었는지 DeepSeek V2를 썼군요.

<english>
ByteDance's code model. The main idea is focusing on LLM based filtering instead of heuristic filters (https://arxiv.org/abs/2412.02595). They used DeepSeek V2, and maybe it means they didn't had prepared model at that time.
</english>

#code #pretraining #corpus #reasoning #rl 