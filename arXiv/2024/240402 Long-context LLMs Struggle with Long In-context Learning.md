https://arxiv.org/abs/2404.02060

*Long-context LLMs Struggle with Long In-context Learning* (Tianle Li, Ge Zhang, Quy Duc Do, Xiang Yue, Wenhu Chen)

> Large Language Models (LLMs) have made significant strides in handling long sequences exceeding 32K tokens. However, their performance evaluation has largely been confined to metrics like perplexity and synthetic tasks, which may not fully capture their abilities in more nuanced, real-world scenarios. This study introduces a specialized benchmark (LIConBench) focusing on long in-context learning within the realm of extreme-label classification. We meticulously selected six datasets with a label range spanning 28 to 174 classes covering different input (few-shot demonstration) length from 2K to 50K. Our benchmark requires LLMs to comprehend the entire input to recognize the massive label spaces to make correct prediction. We evaluate 13 long-context LLMs on our benchmarks. We find that the long-context LLMs perform relatively well under the token length of 20K and the performance benefits from utilizing the long context window. However, after the context window exceeds 20K, most LLMs except GPT-4 will dip dramatically. This suggests a notable gap in current LLM capabilities for processing and understanding long, context-rich sequences. Further analysis revealed a tendency among models to favor predictions for labels presented towards the end at the sequence. Their ability to reason over multiple pieces in the long sequence is yet to be improved. Our study reveals that long context understanding and reasoning is still a challenging task for the existing LLMs. We believe LIConBench could serve as a more realistic evaluation for the future long context LLMs.

Long In-context Learning. 레이블의 수를 늘려서 전체 샘플들을 커버해야만 풀 수 있게 만들고, 각 레이블에 대한 샘플 수를 1 ~ 5개로 세팅해서 Context Length를 변화시키는 방법을 썼습니다.

따라서 Context Length가 길어지는 것에 따라 성능 향상이 있기를 기대하고 있는 세팅이네요. Discovery 과제를 빼고는 GPT-4는 실제로 그런 패턴이 나타나네요.

#in-context-learning #long-context 