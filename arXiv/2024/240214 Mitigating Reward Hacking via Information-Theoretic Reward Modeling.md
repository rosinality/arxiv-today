https://arxiv.org/abs/2402.09345

*Mitigating Reward Hacking via Information-Theoretic Reward Modeling* (Yuchun Miao, Sen Zhang, Liang Ding, Rong Bao, Lefei Zhang, Dacheng Tao)

> Despite the success of reinforcement learning from human feedback (RLHF) in aligning language models with human values, reward hacking, also termed reward overoptimization, remains a critical challenge, which primarily stems from limitations in reward modeling, i.e., generalizability of the reward model and inconsistency in the preference dataset. In this work, we tackle this problem from an information theoretic-perspective, and propose a generalizable and robust framework for reward modeling, namely InfoRM, by introducing a variational information bottleneck objective to filter out irrelevant information and developing a mechanism for model complexity modulation. Notably, we further identify a correlation between overoptimization and outliers in the latent space, establishing InfoRM as a promising tool for detecting reward overoptimization. Inspired by this finding, we propose the Integrated Cluster Deviation Score (ICDS), which quantifies deviations in the latent space, as an indicator of reward overoptimization to facilitate the development of online mitigation strategies. Extensive experiments on a wide range of settings and model scales (70M, 440M, 1.4B, and 7B) support the effectiveness of InfoRM. Further analyses reveal that InfoRM's overoptimization detection mechanism is effective, potentially signifying a notable advancement in the field of RLHF. Code will be released upon acceptance.

Reward Modeling에 Information Bottleneck을 결합시켰군요. 추가로 Overoptimization을 Reward Model의 Information Bottleneck을 사용해 탐지하는 방법을 제안합니다. 클러스터링으로 SFT와 RLHF의 분포의 괴리를 탐지하는 방법이네요.

앞으로도 Reward Overoptimization은 인기 있는 주제일 것 같습니다. 최근 연구들은 보면 기존 딥 러닝 업계에서 Generalization이나 Noisy Label 문제에 대해 시도했던 방법들을 꺼내와서 시도해보고 있다는 느낌이 있네요.

#reward-model #regularization 