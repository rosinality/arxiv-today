https://arxiv.org/abs/2402.00742

*Transforming and Combining Rewards for Aligning Large Language Models* (Zihao Wang, Chirag Nagpal, Jonathan Berant, Jacob Eisenstein, Alex D'Amour, Sanmi Koyejo, Victor Veitch)

> A common approach for aligning language models to human preferences is to first learn a reward model from preference data, and then use this reward model to update the language model. We study two closely related problems that arise in this approach. First, any monotone transformation of the reward model preserves preference ranking; is there a choice that is ``better'' than others? Second, we often wish to align language models to multiple properties: how should we combine multiple reward models? Using a probabilistic interpretation of the alignment procedure, we identify a natural choice for transformation for (the common case of) rewards learned from Bradley-Terry preference models. This derived transformation has two important properties. First, it emphasizes improving poorly-performing outputs, rather than outputs that already score well. This mitigates both underfitting (where some prompts are not improved) and reward hacking (where the model learns to exploit misspecification of the reward model). Second, it enables principled aggregation of rewards by linking summation to logical conjunction: the sum of transformed rewards corresponds to the probability that the output is ``good'' in all measured properties, in a sense we make precise. Experiments aligning language models to be both helpful and harmless using RLHF show substantial improvements over the baseline (non-transformed) approach.

Reward Score에 대한 적절한 단조 변환을 설정할 수 있는가? 그리고 여러 Reward Model을 어떻게 결합할 수 있는가? 라는 문제입니다. 여기서 찾아낸 방법은 logsigmoid와 베이스라인 스코어를 사용하는 방법입니다.

베이스라인을 찾아내는 것이 중요한데 이건 샘플을 여러 개 뽑아서 스코어의 85분위수를 쓰는 방식이나 응답 거부의 스코어를 쓰는 방법을 사용했습니다. 샘플을 여러 개 뽑고 그 샘플들의 Reward 스코어 분포를 본다는 것 자체가 흥미로운 의미를 갖는 것이 아닌가 하는 생각이 드네요.

#reward-model #rlhf 

Can we apply appropriate monotonic transformations on reward score? And how we can combine multiple reward models into on score? This paper suggests to use logsigmoid and baseline score.

It is important to find baseline. This study uses sample multiple responses and use 85th quantile scores or reward score of refusal responses. I think it is interesting to sampling multiple responses and see or utilizing score distribution itself.