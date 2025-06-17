https://arxiv.org/abs/2404.10719

*Is DPO Superior to PPO for LLM Alignment? A Comprehensive Study* (Shusheng Xu, Wei Fu, Jiaxuan Gao, Wenjie Ye, Weilin Liu, Zhiyu Mei, Guangju Wang, Chao Yu, Yi Wu)

> Reinforcement Learning from Human Feedback (RLHF) is currently the most widely used method to align large language models (LLMs) with human preferences. Existing RLHF methods can be roughly categorized as either reward-based or reward-free. Novel applications such as ChatGPT and Claude leverage reward-based methods that first learn a reward model and apply actor-critic algorithms, such as Proximal Policy Optimization (PPO). However, in academic benchmarks, state-of-the-art results are often achieved via reward-free methods, such as Direct Preference Optimization (DPO). Is DPO truly superior to PPO? Why does PPO perform poorly on these benchmarks? In this paper, we first conduct both theoretical and empirical studies on the algorithmic properties of DPO and show that DPO may have fundamental limitations. Moreover, we also comprehensively examine PPO and reveal the key factors for the best performances of PPO in fine-tuning LLMs. Finally, we benchmark DPO and PPO across various a collection of RLHF testbeds, ranging from dialogue to code generation. Experiment results demonstrate that PPO is able to surpass other alignment methods in all cases and achieve state-of-the-art results in challenging code competitions.

PPO가 스스로를 다시 증명해야 하는가 하는 생각이 들긴 합니다만 현재 자체 구축한 데이터셋에서 PPO와 다른 방법들을 비교한 사례는 아주 드물다는 것을 고려하면 그 자체로 의미가 있을 것 같긴 합니다.

여기서 지적하는 DPO의 문제는 OOD 응답을 선호하는 경향이 강하다는 것이네요. 최근 DPO로 인해 길이가 길어지는 문제에 대한 분석에서 (https://arxiv.org/abs/2403.19159) 이 현상이 OOD 문제로 인해 발생하는 것 같다는 추정이 있었죠.

#rlhf

# Links

[[240328 Disentangling Length from Quality in Direct Preference Optimization.md]]