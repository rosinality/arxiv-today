https://arxiv.org/abs/2502.03373

*Demystifying Long Chain-of-Thought Reasoning in LLMs* (Edward Yeo, Yuxuan Tong, Morry Niu, Graham Neubig, Xiang Yue)

> Scaling inference compute enhances reasoning in large language models (LLMs), with long chains-of-thought (CoTs) enabling strategies like backtracking and error correction. Reinforcement learning (RL) has emerged as a crucial method for developing these capabilities, yet the conditions under which long CoTs emerge remain unclear, and RL training requires careful design choices. In this study, we systematically investigate the mechanics of long CoT reasoning, identifying the key factors that enable models to generate long CoT trajectories. Through extensive supervised fine-tuning (SFT) and RL experiments, we present four main findings: (1) While SFT is not strictly necessary, it simplifies training and improves efficiency; (2) Reasoning capabilities tend to emerge with increased training compute, but their development is not guaranteed, making reward shaping crucial for stabilizing CoT length growth; (3) Scaling verifiable reward signals is critical for RL. We find that leveraging noisy, web-extracted solutions with filtering mechanisms shows strong potential, particularly for out-of-distribution (OOD) tasks such as STEM reasoning; and (4) Core abilities like error correction are inherently present in base models, but incentivizing these skills effectively for complex tasks via RL demands significant compute, and measuring their emergence requires a nuanced approach. These insights provide practical guidance for optimizing training strategies to enhance long CoT reasoning in LLMs. Our code is available at: https://github.com/eddycmu/demystify-long-cot.

SFT와 RL을 통한 추론 능력 획득에 대한 분석. 분석들이 많은데 KL Penalty와 생성 길이가 관계가 있을 가능성과 베이스 모델이 프리트레이닝에서 추론 과정에 필요한 능력들을 획득하는 원천이 되었을 가능성이 높은 문서들에 대한 분석이 재미있네요.

특히 포럼 쓰레드들에서 이런 문서를 발견할 가능성이 높다는 것이 흥미롭네요. 한 사람이 작성한 글에서는 사고의 과정이 명시적으로 드러나지 않는 경우가 많지만 여러 사람이 상호작용하는 상황 자체가 하나의 사고의 과정이 될 수 있다는 의미로 생각할 수 있겠습니다. 실용적으로는 이런 포럼 형태의 문서들을 잘 추출하는 것이 추론 능력에 도움이 된다고 생각할 수 있겠네요.

<english>
Analysis on acquiring reasoning capabilities using SFT and RL. There a various analysis, but to me potential relationships between KL penalty and generation length, and analysis on documents that which could be candidate for model to get abilities for reasoning during pretraining.

Especially, I think it is interesting that we can find many such doucments from forum threads. It maybe hard to find explicit thought process from written by individuals, but collective communications between many peoples itself can be a thought process. Practically it may suggest extracting these kind of documents well could be beneficial for reasoning abilities.
</english>

#reasoning #rl 