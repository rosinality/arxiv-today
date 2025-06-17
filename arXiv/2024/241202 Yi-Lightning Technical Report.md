https://arxiv.org/abs/2412.01253

*Yi-Lightning Technical Report* (01.AI: Alan Wake, Albert Wang, Bei Chen, C.X. Lv, Chao Li, Chengen Huang, Chenglin Cai, Chujie Zheng, Daniel Cooper, Ethan Dai, Fan Zhou, Feng Hu, Heng Ji, Howard Qiu, Jiangcheng Zhu, Jun Tian, Katherine Su, Lihuan Zhang, Liying Li, Ming Song, Mou Li, Peng Liu, Qichen Hu, Shawn Wang, Shijun Zhou, Shiyong Li, Tianhang Zhu, Wen Xie, Xiang He, Xiaobo Chen, Xiaohui Hu, Xiaoyi Ren, Xinyao Niu, Yanpeng Li, Yongke Zhao, Yongzhen Luo, Yuchi Xu, Yuxuan Sha, Zhaodong Yan, Zhiyuan Liu, Zirui Zhang)

> This technical report presents Yi-Lightning, our latest flagship large language model (LLM). It achieves exceptional performance, ranking 6th overall on Chatbot Arena, with particularly strong results (2nd to 4th place) in specialized categories including Chinese, Math, Coding, and Hard Prompts. Yi-Lightning leverages an enhanced Mixture-of-Experts (MoE) architecture, featuring advanced expert segmentation and routing mechanisms coupled with optimized KV-caching techniques. Our development process encompasses comprehensive pre-training, supervised fine-tuning (SFT), and reinforcement learning from human feedback (RLHF), where we devise deliberate strategies for multi-stage training, synthetic data construction, and reward modeling. Furthermore, we implement RAISE (Responsible AI Safety Engine), a four-component framework to address safety issues across pre-training, post-training, and serving phases. Empowered by our scalable super-computing infrastructure, all these innovations substantially reduce training, deployment and inference costs while maintaining high-performance standards. With further evaluations on public academic benchmarks, Yi-Lightning demonstrates competitive performance against top-tier LLMs, while we observe a notable disparity between traditional, static benchmark results and real-world, dynamic human preferences. This observation prompts a critical reassessment of conventional benchmarks' utility in guiding the development of more intelligent and powerful AI systems for practical applications. Yi-Lightning is now available through our developer platform at https://platform.lingyiwanwu.com.

Yi-Lightning 테크니컬 리포트. DeepSeekMoE 스타일의 Fine-grained MoE, Sliding window Attention과 Global Attention의 조합, KV 캐시 재사용, DeepSeekMath 스타일의 수학 데이터 수집, In-context Pretraining 등. (https://arxiv.org/abs/2401.06066, https://arxiv.org/abs/2402.03300, https://arxiv.org/abs/2310.10638) 이 방법들이 요즘 일반적인 선택이라는 느낌이군요.

<english>
Technical report of Yi-Lightning. They employed fine-grained MoE in the style of DeepSeekMode, combining sliding window attention and global attention, reusing KV caches, collecting mathematical data following DeepSeekMath, and used in-context pretraining. (https://arxiv.org/abs/2401.06066, https://arxiv.org/abs/2402.03300, https://arxiv.org/abs/2310.10638) These choices are became basic in these days.
</english>

#llm

# Links

[[231016 In-Context Pretraining.md]]
[[240205 DeepSeekMath.md]]
[[240111 DeepSeekMoE.md]]