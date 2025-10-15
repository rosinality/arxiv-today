https://arxiv.org/abs/2510.11370

*Stabilizing MoE Reinforcement Learning by Aligning Training and Inference Routers* (Wenhan Ma, Hailin Zhang, Liang Zhao, Yifan Song, Yudong Wang, Zhifang Sui, Fuli Luo)

> Reinforcement learning (RL) has emerged as a crucial approach for enhancing the capabilities of large language models. However, in Mixture-of-Experts (MoE) models, the routing mechanism often introduces instability, even leading to catastrophic RL training collapse. We analyze the training-inference consistency of MoE models and identify a notable discrepancy in routing behaviors between the two phases. Moreover, even under identical conditions, the routing framework can yield divergent expert selections across repeated forward passes. To address this foundational inconsistency, we propose Rollout Routing Replay (R3), a method that records routing distributions from the inference engine and replays them during training. R3 significantly reduces training-inference policy KL divergence and mitigates extreme discrepancies without compromising training speed. Extensive experiments on various settings confirm that R3 succeeds in stabilizing RL training, preventing collapse and outperforming methods such as GSPO and TIS. We believe this work can offer a new solution for stabilizing RL in MoE models.

학습-추론 갭을 해소하기 위한 MoE 라우팅 리플레이. 자연스럽게 이 라우팅 리플레이는 프리픽스가 공유되어 KV 캐시 Hit이 발생했을 때에 재사용되어야 함.

Routing replay for MoE addresses training-inference gaps in this case. Naturally this routing replay should be reused when prefixes are shared and KV cache hits.

#moe #rl 