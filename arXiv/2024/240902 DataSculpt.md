https://arxiv.org/abs/2409.00997

*DataSculpt: Crafting Data Landscapes for LLM Post-Training through Multi-objective Partitioning* (Keer Lu, Zheng Liang, Xiaonan Nie, Da Pan, Shusen Zhang, Keshi Zhao, Weipeng Chen, Zenan Zhou, Guosheng Dong, Wentao Zhang, Bin Cui)

> The effectiveness of long-context modeling is important for Large Language Models (LLMs) in various applications. Despite their potential, LLMs' efficacy in processing long context does not consistently meet expectations, posing significant challenges for efficient management of prolonged sequences in training. This difficulty is compounded by the scarcity of comprehensive and diverse training datasets suitable for long sequences, which stems from inherent length biases across different data sources, and the logistical complexities associated with massive data management for training in extended contexts. In this work, we introduce DataSculpt, a data construction framework designed to strategically augment the data architecture for extended-context training. Our thorough evaluations demonstrate DataSculpt's remarkable capacity to boost long-context training performance, achieving improvements including an 18.09% increase in retrieval augmentation, 21.23% in summarization, 21.27% in reading comprehension, and a 3.81% rise in code completion, all while preserving the models' overall proficiency with a 4.88% improvement.

Long Context 학습 쪽의 문제군요. Long Context 데이터는 대부분 서적 등에 많으니 웹 데이터 등에 대해서는 도메인 불균형이 있다, 따라서 In-context Pretraining처럼 (https://arxiv.org/abs/2310.10638) 샘플을 잘 연결하는 방법을 사용하자, 이런 아이디어입니다.

다만 Llama 3에서는 Long Context 학습에 Attention Masking을 쓰는 쪽이 나았다고 하죠. 이 부분을 고려해야 할 것 같습니다.

#long-context #pretraining

# Links

[[231016 In-Context Pretraining.md]]