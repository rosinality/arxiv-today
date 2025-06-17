https://arxiv.org/abs/2407.16008

*Boosting Reward Model with Preference-Conditional Multi-Aspect Synthetic Data Generation* (Jiaming Shen, Ran Xu, Yennie Jun, Zhen Qin, Tianqi Liu, Carl Yang, Yi Liang, Simon Baumgartner, Michael Bendersky)

> Reward models (RMs) are crucial for aligning large language models (LLMs) with human preferences. They are trained using preference datasets where each example consists of one input prompt, two responses, and a preference label. As curating a high-quality human labeled preference dataset is both time-consuming and expensive, people often rely on existing powerful LLMs for preference label generation. This can potentially introduce noise and impede RM training. In this work, we present RMBoost, a novel synthetic preference data generation paradigm to boost reward model quality. Unlike traditional methods, which generate two responses before obtaining the preference label, RMBoost first generates one response and selects a preference label, followed by generating the second more (or less) preferred response conditioned on the pre-selected preference label and the first response. This approach offers two main advantages. First, RMBoost reduces labeling noise since preference pairs are constructed intentionally. Second, RMBoost facilitates the creation of more diverse responses by incorporating various quality aspects (e.g., helpfulness, relevance, completeness) into the prompts. We conduct extensive experiments across three diverse datasets and demonstrate that RMBoost outperforms other synthetic preference data generation techniques and significantly boosts the performance of four distinct reward models.

모델로 응답을 샘플링한 다음 Preference Label을 하나 정해서 Preference Label을 Condition을 주고 Rewriting한 응답을 Preference Pair로 사용하는 방식. 즉 주어진 응답보다 나은/못한 응답을 재작성으로 만들어내는 방식이네요.

Llama 3가 정말 온갖 방법으로 Synthetic Preference를 만들어내는 사례를 보여줬죠. (물론 LLM Judge가 주된 방법이긴 합니다만) 이런 형태의 Synthetic Preference 방법들을 다시 생각해보면 재미있을 듯 하네요.

#rlaif #alignment 