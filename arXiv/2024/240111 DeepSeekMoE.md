https://arxiv.org/abs/2401.06066

*DeepSeekMoE: Towards Ultimate Expert Specialization in Mixture-of-Experts Language Models* (Damai Dai, Chengqi Deng, Chenggang Zhao, R.X. Xu, Huazuo Gao, Deli Chen, Jiashi Li, Wangding Zeng, Xingkai Yu, Y. Wu, Zhenda Xie, Y.K. Li, Panpan Huang, Fuli Luo, Chong Ruan, Zhifang Sui, Wenfeng Liang)

> In the era of large language models, Mixture-of-Experts (MoE) is a promising architecture for managing computational costs when scaling up model parameters. However, conventional MoE architectures like GShard, which activate the top-$K$ out of $N$ experts, face challenges in ensuring expert specialization, i.e. each expert acquires non-overlapping and focused knowledge. In response, we propose the DeepSeekMoE architecture towards ultimate expert specialization. It involves two principal strategies: (1) finely segmenting the experts into $mN$ ones and activating $mK$ from them, allowing for a more flexible combination of activated experts; (2) isolating $K_s$ experts as shared ones, aiming at capturing common knowledge and mitigating redundancy in routed experts. Starting from a modest scale with 2B parameters, we demonstrate that DeepSeekMoE 2B achieves comparable performance with GShard 2.9B, which has 1.5 times the expert parameters and computation. In addition, DeepSeekMoE 2B nearly approaches the performance of its dense counterpart with the same number of total parameters, which set the upper bound of MoE models. Subsequently, we scale up DeepSeekMoE to 16B parameters and show that it achieves comparable performance with LLaMA2 7B, with only about 40% of computations. Further, our preliminary efforts to scale up DeepSeekMoE to 145B parameters consistently validate its substantial advantages over the GShard architecture, and show its performance comparable with DeepSeek 67B, using only 28.5% (maybe even 18.2%) of computations.

예고됐었던 DeepSeek MoE가 나왔네요. 7B Dense 모델 정도의 성능을 타겟했군요. 흥미로운 부분은 Expert를 쪼개서 더 작은 Expert를 더 많이 활성화시키려고 했다는 것입니다. Expert의 조합의 다양성을 높여서 여러 Expert들을 동시에 활용할 수 있게 하고, 공유되는 Expert를 만들어서 Expert들이 같은 지식을 중복적으로 인코딩하는 것을 방지하려고 시도했습니다.

논문에서는 이 모델 선택이 GShard 같은 세팅보다 효과적이었다고 이야기 하고 있네요. 여러모로 MoE 모델들에 대한 Scaling Law를 다시 분석하는 것이 필요해진 것 같습니다. (https://arxiv.org/abs/2202.01169)

145B 모델을 만들고 있다고 하는데 이쪽의 퍼포먼스도 기대가 되는군요.

#moe #llm

# Links

[[220202 Unified Scaling Laws for Routed Language Models.md]]