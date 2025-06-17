https://arxiv.org/abs/2406.06326

*Self-Tuning: Instructing LLMs to Effectively Acquire New Knowledge through Self-Teaching* (Xiaoying Zhang, Baolin Peng, Ye Tian, Jingyan Zhou, Yipeng Zhang, Haitao Mi, Helen Meng)

> Large language models (LLMs) often struggle to provide up-to-date information due to their one-time training and the constantly evolving nature of the world. To keep LLMs current, existing approaches typically involve continued pre-training on new documents. However, they frequently face difficulties in extracting stored knowledge. Motivated by the remarkable success of the Feynman Technique in efficient human learning, we introduce Self-Tuning, a learning framework aimed at improving an LLM's ability to effectively acquire new knowledge from raw documents through self-teaching. Specifically, we develop a Self-Teaching strategy that augments the documents with a set of knowledge-intensive tasks created in a self-supervised manner, focusing on three crucial aspects: memorization, comprehension, and self-reflection. Additionally, we introduce three Wiki-Newpages-2023-QA datasets to facilitate an in-depth analysis of an LLM's knowledge acquisition ability concerning memorization, extraction, and reasoning. Extensive experimental results on Llama2 family models reveal that Self-Tuning consistently exhibits superior performance across all knowledge acquisition tasks and excels in preserving previous knowledge.

QA 데이터를 의도적으로 사용해서 모델의 학습을 가속하는 접근의 확장 버전 (https://arxiv.org/abs/2402.12847) 여기에서는 추가적인 과제를 더 도입했네요.

프리트레이닝 데이터에 Instruction 데이터를 사용하는 사례처럼 이런 추가적인 과제의 활용이 실질적인 성능 향상으로 이어지는지의 여부가 중요한 문제이긴 할 듯 합니다. 다만 일종의 학습 Objective로 보면 의미가 있을 수 있겠다는 생각이 드네요.

#pretraining

# Links

[[240220 Instruction-tuned Language Models are Better Knowledge Learners.md]]