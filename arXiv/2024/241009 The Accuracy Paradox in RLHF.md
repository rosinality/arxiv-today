https://arxiv.org/abs/2410.06554

*The Accuracy Paradox in RLHF: When Better Reward Models Don't Yield Better Language Models* (Yanjun Chen, Dawei Zhu, Yirong Sun, Xinghao Chen, Wei Zhang, Xiaoyu Shen)

> Reinforcement Learning from Human Feedback significantly enhances Natural Language Processing by aligning language models with human expectations. A critical factor in this alignment is the strength of reward models used during training. This study explores whether stronger reward models invariably lead to better language models. In this paper, through experiments on relevance, factuality, and completeness tasks using the QA-FEEDBACK dataset and reward models based on Longformer, we uncover a surprising paradox: language models trained with moderately accurate reward models outperform those guided by highly accurate ones. This challenges the widely held belief that stronger reward models always lead to better language models, and opens up new avenues for future research into the key factors driving model performance and how to choose the most suitable reward models. Code and additional details are available at [https://github.com/EIT-NLP/AccuracyParadox-RLHF](https://github.com/EIT-NLP/AccuracyParadox-RLHF).

정확도가 더 높은 Reward Model이 더 나은 RLHF 결과로 이어지지 않는다는 결과. Reward Model의 역할을 생각하면 정확도 이상으로 Reward Score의 거동과 특성이 중요하겠죠.

<english>
Result that more accurate reward model does not result in better RLHF results. If we think about the role of reward model then characteristics of reward score could be important than mere accuracy.
</english>

#reward-model 