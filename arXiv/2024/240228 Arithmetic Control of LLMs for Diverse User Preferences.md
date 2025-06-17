https://arxiv.org/abs/2402.18571

*Arithmetic Control of LLMs for Diverse User Preferences: Directional Preference Alignment with Multi-Objective Rewards* (Haoxiang Wang, Yong Lin, Wei Xiong, Rui Yang, Shizhe Diao, Shuang Qiu, Han Zhao, Tong Zhang)

> Fine-grained control over large language models (LLMs) remains a significant challenge, hindering their adaptability to diverse user needs. While Reinforcement Learning from Human Feedback (RLHF) shows promise in aligning LLMs, its reliance on scalar rewards often limits its ability to capture diverse user preferences in real-world applications. To address this limitation, we introduce the Directional Preference Alignment (DPA) framework. Unlike the scalar-reward RLHF, DPA incorporates multi-objective reward modeling to represent diverse preference profiles. Additionally, DPA models user preferences as directions (i.e., unit vectors) in the reward space to achieve user-dependent preference control. Our method involves training a multi-objective reward model and then fine-tuning the LLM with a preference-conditioned variant of Rejection Sampling Finetuning (RSF), an RLHF method adopted by Llama 2. This method enjoys a better performance trade-off across various reward objectives. In comparison with the scalar-reward RLHF, DPA offers users intuitive control over LLM generation: they can arithmetically specify their desired trade-offs (e.g., more helpfulness with less verbosity). We also validate the effectiveness of DPA with real-world alignment experiments on Mistral-7B. Our method provides straightforward arithmetic control over the trade-off between helpfulness and verbosity while maintaining competitive performance with strong baselines such as Direct Preference Optimization (DPO).

SteerLM (https://arxiv.org/abs/2310.05344) 처럼 조작 가능한 슬라이더를 제공하는 모델 개발. 여기서는 유저의 선호를 Unit Vector로 본다는 것이 특징이네요. 즉 방향을 선택하는 것이죠. 이 Unit Vector를 사용해 Reward Score를 결합합니다.

이건 Helpfulness와 Conciseness 같이 종종 충돌하는 측면을 결합할 때 자연스러울 수 있을 것 같긴 합니다. 그런데 아주 독립적인 경우는 어떨지 궁금하긴 하네요.

시스템 프롬프트 측면에서 흥미로운 질문인 것 같긴 합니다.

#alignment

# Links

