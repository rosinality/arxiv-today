https://arxiv.org/abs/2510.23027

*Towards Stable and Effective Reinforcement Learning for Mixture-of-Experts* (Di Zhang, Xun Wu, Shaohan Huang, Yaru Hao, Li Dong, Zewen Chi, Zhifang Sui, Furu Wei)

> Recent advances in reinforcement learning (RL) have substantially improved the training of large-scale language models, leading to significant gains in generation quality and reasoning ability. However, most existing research focuses on dense models, while RL training for Mixture-of-Experts (MoE) architectures remains underexplored. To address the instability commonly observed in MoE training, we propose a novel router-aware approach to optimize importance sampling (IS) weights in off-policy RL. Specifically, we design a rescaling strategy guided by router logits, which effectively reduces gradient variance and mitigates training divergence. Experimental results demonstrate that our method significantly improves both the convergence stability and the final performance of MoE models, highlighting the potential of RL algorithmic innovations tailored to MoE architectures and providing a promising direction for efficient training of large-scale expert models.

MoE RL 안정화에 대한 또 다른 연구. 여기서는 Routing Score가 크게 바뀐 토큰을 Downweight. IcePop과 비슷한 효과일지도?

More work on stabilization of MoE in RL. This work downweights tokens that had a larger shift in routing scores. Maybe it has similar effects to IcePop?

#rl #moe 