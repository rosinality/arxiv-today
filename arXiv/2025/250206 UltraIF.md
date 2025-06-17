https://arxiv.org/abs/2502.04153

*UltraIF: Advancing Instruction Following from the Wild* (Kaikai An, Li Sheng, Ganqu Cui, Shuzheng Si, Ning Ding, Yu Cheng, Baobao Chang)

> Instruction-following made modern large language models (LLMs) helpful assistants. However, the key to taming LLMs on complex instructions remains mysterious, for that there are huge gaps between models trained by open-source community and those trained by leading companies. To bridge the gap, we propose a simple and scalable approach UltraIF for building LLMs that can follow complex instructions with open-source data. UltraIF first decomposes real-world user prompts into simpler queries, constraints, and corresponding evaluation questions for the constraints. Then, we train an UltraComposer to compose constraint-associated prompts with evaluation questions. This prompt composer allows us to synthesize complicated instructions as well as filter responses with evaluation questions. In our experiment, for the first time, we successfully align LLaMA-3.1-8B-Base to catch up with its instruct version on 5 instruction-following benchmarks without any benchmark information, using only 8B model as response generator and evaluator. The aligned model also achieved competitive scores on other benchmarks. Moreover, we also show that UltraIF could further improve LLaMA-3.1-8B-Instruct through self-alignment, motivating broader use cases for the method. Our code will be available at https://github.com/kkk-an/UltraIF.

Instruction Following 능력을 위한 데이터 구축. 사용자의 지시를 단순화된 지시와 제약 조건으로 분해하고 평가를 위한 질문을 생성. 그리고 단순화된 지시에서 사용자의 지시와 제약 조건을 생성하는 것을 반복하는 것으로 복잡도를 높이는군요.

<english>
Building dataset for instruction following capacity. Decompose user's instruction into simplified instruction and constraints, and then generate questions for evaluation. And increasing complexity of instructions by iteratively generate of user's input and constraints from simplified instructions.
</english>

#synthetic-data #instruction-tuning 