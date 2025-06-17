https://arxiv.org/abs/2402.03300

*DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models* (Zhihong Shao, Peiyi Wang, Qihao Zhu, Runxin Xu, Junxiao Song, Mingchuan Zhang, Y.K. Li, Y. Wu, Daya Guo)

> Mathematical reasoning poses a significant challenge for language models due to its complex and structured nature. In this paper, we introduce DeepSeekMath 7B, which continues pre-training DeepSeek-Coder-Base-v1.5 7B with 120B math-related tokens sourced from Common Crawl, together with natural language and code data. DeepSeekMath 7B has achieved an impressive score of 51.7% on the competition-level MATH benchmark without relying on external toolkits and voting techniques, approaching the performance level of Gemini-Ultra and GPT-4. Self-consistency over 64 samples from DeepSeekMath 7B achieves 60.9% on MATH. The mathematical reasoning capability of DeepSeekMath is attributed to two key factors: First, we harness the significant potential of publicly available web data through a meticulously engineered data selection pipeline. Second, we introduce Group Relative Policy Optimization (GRPO), a variant of Proximal Policy Optimization (PPO), that enhances mathematical reasoning abilities while concurrently optimizing the memory usage of PPO.

DeepSeek의 수학 모델. OpenWebMath를 기반으로 유사한 문서를 찾는 방식으로 데이터 구축 + 추가적으로 관련된 도메인을 발굴하는 방식으로 데이터를 확보했습니다. 이렇게 구축한 데이터셋으로 기존 데이터보다 더 나은 성능을 확보했습니다. (크기 자체도 크긴 하지만요.)

여기서 코드 학습이 수학 성능에 도움이 된다는 것, arXiv 데이터는 그대로는 도움이 되지 않는 것 같다는 것을 발견했습니다.

추가적으로 SFT와 RL 실험을 했는데 RL 실험의 비중이 크네요. 일단 Value function을 빼버리고 여러 샘플에 대한 Reward 평균으로 대체한 GRPO를 사용했습니다. 여기에 MathShepherd (https://arxiv.org/abs/2312.08935) 로 데이터를 생성해서 Process Supervision을 줬네요. Online vs Offline, 1-0 vs Reward Score, Iterative RL 등에 대한 실험도 했습니다.

#math #llm 

Math model of DeepSeek! They constructed math data by find out similar documents to OpenWebMath, and mining related URL domains. They shows that this data is better than previous data in terms of the performance. (Though their data is significantly larger.)

They found that training on code data is beneficial to math performances, and arXiv data is seems like not beneficial in current settings.

Additionally they did SFT and RL experiments, and much of the paper is devoted to RL results. They used GRPO which removes value function from PPO and replace it with average reward of multiple samples. They used MathShepherd to generate data and did process supervision. They also compared online vs offline methods, using 1-0 or reward score, and iterative rl.

# Links

[[231214 Math-Shepherd.md]]