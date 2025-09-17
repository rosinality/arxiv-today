https://arxiv.org/abs/2508.04117

*Unveiling Over-Memorization in Finetuning LLMs for Reasoning Tasks* (Zhiwen Ruan, Yun Chen, Yutao Hou, Peng Li, Yang Liu, Guanhua Chen)

> The pretrained large language models (LLMs) are finetuned with labeled data for better instruction following ability and alignment with human values. In this paper, we study the learning dynamics of LLM finetuning on reasoning tasks and reveal the uncovered over-memorization phenomenon during a specific stage of LLM finetuning. At this stage, the LLMs have excessively memorized training data and exhibit high test perplexity while maintaining good test accuracy. We investigate the conditions that lead to LLM over-memorization and find that training epochs and large learning rates contribute to this issue. Although models with over-memorization demonstrate comparable test accuracy to normal models, they suffer from reduced robustness, poor out-of-distribution generalization, and decreased generation diversity. Our experiments unveil the over-memorization to be broadly applicable across different tasks, models, and finetuning methods. Our research highlights that overparameterized, extensively finetuned LLMs exhibit unique learning dynamics distinct from traditional machine learning models. Based on our observations of over-memorization, we provide recommendations on checkpoint and learning rate selection during finetuning.

파인튜닝 진행에 따라 테스트 정확도와 테스트 Perplexity가 같이 상승하는 현상에 대한 분석. 사실 일반적이고 높은 테스트 정확도를 노리기 위해 의도적으로 사용되는 경우도 있지만 여기서는 그것이 OOD 성능과 샘플 다양성에 좋지 않다는 주장이 중요할 듯. 마찬가지로 SFT와 관련된 기본적인 문제.

The analysis on the phenomenon where test accuracy and perplexity go up together during finetuning. This is actually a common thing and sometimes intentionally tolerated to achieve higher test accuracy. But the key point of this study is that this phenomenon can be harmful to OOD and sample diversity. And this is also a basic problem in SFT.

#generalization 