https://arxiv.org/abs/2404.15045

*Multi-Head Mixture-of-Experts* (Xun Wu, Shaohan Huang, Wenhui Wang, Furu Wei)

> Sparse Mixtures of Experts (SMoE) scales model capacity without significant increases in training and inference costs, but exhibits the following two issues: (1) Low expert activation, where only a small subset of experts are activated for optimization. (2) Lacking fine-grained analytical capabilities for multiple semantic concepts within individual tokens. We propose Multi-Head Mixture-of-Experts (MH-MoE), which employs a multi-head mechanism to split each token into multiple sub-tokens. These sub-tokens are then assigned to and processed by a diverse set of experts in parallel, and seamlessly reintegrated into the original token form. The multi-head mechanism enables the model to collectively attend to information from various representation spaces within different experts, while significantly enhances expert activation, thus deepens context understanding and alleviate overfitting. Moreover, our MH-MoE is straightforward to implement and decouples from other SMoE optimization methods, making it easy to integrate with other SMoE models for enhanced performance. Extensive experimental results across three tasks: English-focused language modeling, Multi-lingual language modeling and Masked multi-modality modeling tasks, demonstrate the effectiveness of MH-MoE.

MoE에서 토큰 임베딩을 쪼개고 각 임베딩마다 Top-K개의 Expert로 라우팅 되도록 만든 디자인. 사용하는 Expert의 다양성, 특히 개별 토큰에 대해 사용하는 Expert의 다양성을 높인다는 아이디어군요. 작은 Expert의 더 다양한 조합을 사용한다는 요즘 유행과 잘 맞지 않나 싶습니다.

#moe 