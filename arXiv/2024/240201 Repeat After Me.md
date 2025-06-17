https://arxiv.org/abs/2402.01032

*Repeat After Me: Transformers are Better than State Space Models at Copying* (Samy Jelassi, David Brandfonbrener, Sham M. Kakade, Eran Malach)

> Transformers are the dominant architecture for sequence modeling, but there is growing interest in models that use a fixed-size latent state that does not depend on the sequence length, which we refer to as "generalized state space models" (GSSMs). In this paper we show that while GSSMs are promising in terms of inference-time efficiency, they are limited compared to transformer models on tasks that require copying from the input context. We start with a theoretical analysis of the simple task of string copying and prove that a two layer transformer can copy strings of exponential length while GSSMs are fundamentally limited by their fixed-size latent state. Empirically, we find that transformers outperform GSSMs in terms of efficiency and generalization on synthetic tasks that require copying the context. Finally, we evaluate pretrained large language models and find that transformer models dramatically outperform state space models at copying and retrieving information from context. Taken together, these results suggest a fundamental gap between transformers and GSSMs on tasks of practical interest.

트랜스포머와 State Space Model의 Copy 과제, 즉 입력 시퀀스를 재현하는 과제에 대한 성능 비교. 사실상 Associative Recall과 관련된 과제죠. 트랜스포머가 Mamba에 비해 더 샘플 효율적이고 ALiBi, 혹은 이전 n개 토큰에 대해서만 Bias가 0이고 그 외에는 마스킹하는 주는 Hard ALiBi를 적용하면 Length Generalization도 발생합니다.

State Space Model의 뚜렷한 문제이고 이 문제를 해소하는가가 중요한 고려 사항이죠. State Space Model이 가지는 또 다른 한계가 있을지도 흥미로운 부분일 듯 합니다. 만약 없다고 한다면 바로 State Space Model을 학습시키러 가야겠죠.

#state-space-model #transformer 

Comparison of transformers and state-space models on copy task, that is, reconstructing the input sequences. Actually it is related to associative recall task. This study shows that transformer is more sample efficient, and if ALiBi or Hard ALiBi, which masks tokens beyond n and set bias to 0 if it is in window of n, length generalization could be achieved.

This is apparent problem of state space models, and it is important to resolve this. It could be also interesting is there are crucial problems of state space models. If there not, then we should go to train state space models immediately.