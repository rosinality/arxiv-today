https://arxiv.org/abs/2501.09368

*Aligning Instruction Tuning with Pre-training* (Yiming Liang, Tianyu Zheng, Xinrun Du, Ge Zhang, Xingwei Qu, Xiang Yue, Chujie Zheng, Jiaheng Liu, Lei Ma, Wenhu Chen, Guoyin Wang, Zhaoxiang Zhang, Wenhao Huang, Jiajun Zhang)

> Instruction tuning enhances large language models (LLMs) to follow human instructions across diverse tasks, relying on high-quality datasets to guide behavior. However, these datasets, whether manually curated or synthetically generated, are often narrowly focused and misaligned with the broad distributions captured during pre-training, limiting LLM generalization and effective use of pre-trained knowledge. We propose *Aligning Instruction Tuning with Pre-training* (AITP), a method that bridges this gap by identifying coverage shortfalls in instruction-tuning datasets and rewriting underrepresented pre-training data into high-quality instruction-response pairs. This approach enriches dataset diversity while preserving task-specific objectives. Evaluations on three fully open LLMs across eight benchmarks demonstrate consistent performance improvements with AITP. Ablations highlight the benefits of adaptive data selection, controlled rewriting, and balanced integration, emphasizing the importance of aligning instruction tuning with pre-training distributions to unlock the full potential of LLMs.

프리트레이닝 데이터셋 중 SFT 데이터셋이 커버하지 못하는 영역을 발굴해서 그 데이터셋들을 QA 데이터로 전환한다는 아이디어. QA라는 단일 과제를 넘어서 과제들을 확장하는 방향으로 나아가면 더 재미있을 듯 하네요.

<english>
The idea that mining area of distribution in pretraining datasets not covered by SFT datasets and transform it into QA data. It would be more interesting if we can generalize it for non-covered tasks instead single task like QA.
</english>

#instruction-tuning 