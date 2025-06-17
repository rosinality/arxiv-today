https://arxiv.org/abs/2403.15796

*Understanding Emergent Abilities of Language Models from the Loss Perspective* (Zhengxiao Du, Aohan Zeng, Yuxiao Dong, Jie Tang)

> Recent studies have put into question the belief that emergent abilities in language models are exclusive to large models. This skepticism arises from two observations: 1) smaller models can also exhibit high performance on emergent abilities and 2) there is doubt on the discontinuous metrics used to measure these abilities. In this paper, we propose to study emergent abilities in the lens of pre-training loss, instead of model size or training compute. We demonstrate that the models with the same pre-training loss, but different model and data sizes, generate the same performance on various downstream tasks. We also discover that a model exhibits emergent abilities on certain tasks -- regardless of the continuity of metrics -- when its pre-training loss falls below a specific threshold. Before reaching this threshold, its performance remains at the level of random guessing. This inspires us to redefine emergent abilities as those that manifest in models with lower pre-training losses, highlighting that these abilities cannot be predicted by merely extrapolating the performance trends of models with higher pre-training losses.

LLM의 Emergent Behavior 문제. (https://arxiv.org/abs/2206.07682, https://arxiv.org/abs/2304.15004) 직접 다양한 모델을 다양한 토큰 수에 대해 학습시킨 다음 Loss에 따른 성능 그래프를 그렸습니다. Brier Score 같은 연속적인 척도를 사용하는 경우에도 그래프에서 Elbow가 나타납니다.

#scaling-law #llm

# Links

