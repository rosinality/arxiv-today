https://arxiv.org/abs/2509.20186

*Thinking Augmented Pre-training* (Liang Wang, Nan Yang, Shaohan Huang, Li Dong, Furu Wei)

> This paper introduces a simple and scalable approach to improve the data efficiency of large language model (LLM) training by augmenting existing text data with thinking trajectories. The compute for pre-training LLMs has been growing at an unprecedented rate, while the availability of high-quality data remains limited. Consequently, maximizing the utility of available data constitutes a significant research challenge. A primary impediment is that certain high-quality tokens are difficult to learn given a fixed model capacity, as the underlying rationale for a single token can be exceptionally complex and deep. To address this issue, we propose Thinking augmented Pre-Training (TPT), a universal methodology that augments text with automatically generated thinking trajectories. Such augmentation effectively increases the volume of the training data and makes high-quality tokens more learnable through step-by-step reasoning and decomposition. We apply TPT across diverse training configurations up to $100$B tokens, encompassing pre-training with both constrained and abundant data, as well as mid-training from strong open-source checkpoints. Experimental results indicate that our method substantially improves the performance of LLMs across various model sizes and families. Notably, TPT enhances the data efficiency of LLM pre-training by a factor of $3$. For a $3$B parameter model, it improves the post-training performance by over $10\%$ on several challenging reasoning benchmarks.

프리트레이닝 코퍼스에 사고 궤적을 부착. 아주 단순하게 프롬프팅으로 해결. OpenAI는 분명히 이런 접근을 시도했을 텐데, 성공적이었을지?

Attaching thinking trajectories to the pretraining corpus. They did this simply by prompting. I believe OpenAI definitely tried to synthesize these data. Were they successful?

#synthetic-data 