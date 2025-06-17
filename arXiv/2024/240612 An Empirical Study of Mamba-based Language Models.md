https://arxiv.org/abs/2406.07887

*An Empirical Study of Mamba-based Language Models* (Roger Waleffe, Wonmin Byeon, Duncan Riach, Brandon Norick, Vijay Korthikanti, Tri Dao, Albert Gu, Ali Hatamizadeh, Sudhakar Singh, Deepak Narayanan, Garvit Kulshreshtha, Vartika Singh, Jared Casper, Jan Kautz, Mohammad Shoeybi, Bryan Catanzaro)

> Selective state-space models (SSMs) like Mamba overcome some of the shortcomings of Transformers, such as quadratic computational complexity with sequence length and large inference-time memory requirements from the key-value cache. Moreover, recent studies have shown that SSMs can match or exceed the language modeling capabilities of Transformers, making them an attractive alternative. In a controlled setting (e.g., same data), however, studies so far have only presented small scale experiments comparing SSMs to Transformers. To understand the strengths and weaknesses of these architectures at larger scales, we present a direct comparison between 8B-parameter Mamba, Mamba-2, and Transformer models trained on the same datasets of up to 3.5T tokens. We also compare these models to a hybrid architecture consisting of 43% Mamba-2, 7% attention, and 50% MLP layers (Mamba-2-Hybrid). Using a diverse set of tasks, we answer the question of whether Mamba models can match Transformers at larger training budgets. Our results show that while pure SSMs match or exceed Transformers on many tasks, they lag behind Transformers on tasks which require strong copying or in-context learning abilities (e.g., 5-shot MMLU, Phonebook) or long-context reasoning. In contrast, we find that the 8B Mamba-2-Hybrid exceeds the 8B Transformer on all 12 standard tasks we evaluated (+2.65 points on average) and is predicted to be up to 8x faster when generating tokens at inference time. To validate long-context capabilities, we provide additional experiments evaluating variants of the Mamba-2-Hybrid and Transformer extended to support 16K, 32K, and 128K sequences. On an additional 23 long-context tasks, the hybrid model continues to closely match or exceed the Transformer on average. To enable further study, we release the checkpoints as well as the code used to train our models as part of NVIDIA's Megatron-LM project.

NVIDIA 쪽에서 Mamba와 Mamba-2 (https://arxiv.org/abs/2405.21060), 그리고 하이브리드 모델에 대한 학습과 평가를 진행했군요. Megatron-LM에도 코드가 릴리즈 됐다고 합니다.

Mamba 단독으로는 어렵다는 것을 재발견 했고 하이브리드 모델은 트랜스포머를 거의 따라잡거나 상회할 수 있다는 것을 확인했습니다. 다만 하이브리드 모델이 맥락에 민감하다는 것, 즉 맥락에 맞지 않는 텍스트들이 들어간 경우나 프롬프트의 포맷 등에 민감하다는 것을 발견했네요. 관계 없는 문서들을 이어붙여 시퀀스 길이를 채우는 일반적인 학습 방법이 SSM에는 안 맞을 수도 있을 것 같다는 이야기를 합니다. 상태 리셋 같은 것이 필요할지도 모르겠네요.

#state-space-model

# Links

[[240531 Transformers are SSMs.md]]