https://arxiv.org/abs/2406.10216

*Regularizing Hidden States Enables Learning Generalizable Reward Model for LLMs* (Rui Yang, Ruomeng Ding, Yong Lin, Huan Zhang, Tong Zhang)

> Reward models trained on human preference data have been proven to be effective for aligning Large Language Models (LLMs) with human intent within the reinforcement learning from human feedback (RLHF) framework. However, the generalization capabilities of current reward models to unseen prompts and responses are limited. This limitation can lead to an unexpected phenomenon known as reward over-optimization, where excessive optimization of rewards results in a decline in actual performance. While previous research has advocated for constraining policy optimization, our study proposes a novel approach to enhance the reward model's generalization ability against distribution shifts by regularizing the hidden states. Specifically, we retain the base model's language model head and incorporate a suite of text-generation losses to preserve the hidden states' text generation capabilities, while concurrently learning a reward head behind the same hidden states. Our experimental results demonstrate that the introduced regularization technique markedly improves the accuracy of learned reward models across a variety of out-of-distribution (OOD) tasks and effectively alleviate the over-optimization issue in RLHF, offering a more reliable and robust preference learning paradigm.

Reward Model 학습 과정에서 LM 헤드를 사용해 Autoregressive Loss를 추가시키면 좋다는 결과. Anthropic (https://arxiv.org/abs/2112.00861) 에서도 비슷한 트릭을 사용했었죠. Preference 데이터의 규모가 커지고 있다는 것을 고려하면 Reward Model에도 프리트레이닝 Loss 같은 요소가 필요할 것 같긴 합니다.

#reward-model

# Links

[[230628 A General Language Assistant as a Laboratory for Alignment.md]]