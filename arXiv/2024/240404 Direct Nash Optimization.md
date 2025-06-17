https://arxiv.org/abs/2404.03715

*Direct Nash Optimization: Teaching Language Models to Self-Improve with General Preferences* (Corby Rosset, Ching-An Cheng, Arindam Mitra, Michael Santacroce, Ahmed Awadallah, Tengyang Xie)

> This paper studies post-training large language models (LLMs) using preference feedback from a powerful oracle to help a model iteratively improve over itself. The typical approach for post-training LLMs involves Reinforcement Learning from Human Feedback (RLHF), which traditionally separates reward learning and subsequent policy optimization. However, such a reward maximization approach is limited by the nature of "point-wise" rewards (such as Bradley-Terry model), which fails to express complex intransitive or cyclic preference relations. While advances on RLHF show reward learning and policy optimization can be merged into a single contrastive objective for stability, they yet still remain tethered to the reward maximization framework. Recently, a new wave of research sidesteps the reward maximization presumptions in favor of directly optimizing over "pair-wise" or general preferences. In this paper, we introduce Direct Nash Optimization (DNO), a provable and scalable algorithm that marries the simplicity and stability of contrastive learning with theoretical generality from optimizing general preferences. Because DNO is a batched on-policy algorithm using a regression-based objective, its implementation is straightforward and efficient. Moreover, DNO enjoys monotonic improvement across iterations that help it improve even over a strong teacher (such as GPT-4). In our experiments, a resulting 7B parameter Orca-2.5 model aligned by DNO achieves the state-of-the-art win-rate against GPT-4-Turbo of 33% on AlpacaEval 2.0 (even after controlling for response length), an absolute gain of 26% (7% to 33%) over the initializing model. It outperforms models with far more parameters, including Mistral Large, Self-Rewarding LM (70B parameters), and older versions of GPT-4.

Nash Learning (https://arxiv.org/abs/2312.00886) 을 단순화한 알고리즘이군요. Online Response를 샘플링한 다음 Preference 함수로 랭킹하고 가장 순위 차이가 많이 나는 페어를 사용해 DPO를 합니다. West-of-N (https://arxiv.org/abs/2401.12086) 을 생각나게 하는 부분이 있네요.

결과적으로 GPT-4로 랭킹을 반복적으로 획득한 다음 GPT-4로 평가하는 패턴이긴 합니다.

#rlhf

# Links

[[231201 Nash Learning from Human Feedback.md]]
[[240122 West-of-N.md]]