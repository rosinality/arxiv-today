https://arxiv.org/abs/2503.24067

*TransMamba: Flexibly Switching between Transformer and Mamba* (Yixing Li, Ruobing Xie, Zhen Yang, Xingwu Sun, Shuaipeng Li, Weidong Han, Zhanhui Kang, Yu Cheng, Chengzhong Xu, Di Wang, Jie Jiang)

> Transformers are the cornerstone of modern large language models, but their quadratic computational complexity limits efficiency in long-sequence processing. Recent advancements in Mamba, a state space model (SSM) with linear complexity, offer promising efficiency gains but suffer from unstable contextual learning and multitask generalization. This paper proposes TransMamba, a novel framework that unifies Transformer and Mamba through shared parameter matrices (e.g., QKV and CBx), and thus could dynamically switch between attention and SSM mechanisms at different token lengths and layers. We design the Memory converter to bridge Transformer and Mamba by converting attention outputs into SSM-compatible states, ensuring seamless information flow at TransPoints where the transformation happens. The TransPoint scheduling is also thoroughly explored for further improvements. We conducted extensive experiments demonstrating that TransMamba achieves superior training efficiency and performance compared to baselines, and validated the deeper consistency between Transformer and Mamba paradigms, offering a scalable solution for next-generation sequence modeling.

Attention과 SSM의 레이어 간 결합, 레이어 내 결합에 (https://arxiv.org/abs/2411.13676) 이어 시퀀스 내 결합까지 등장했네요. 시퀀스 내에서 Attention에서 Mamba로 전환하는 방법입니다.

<english>
Beyond inter-layer combination of attention and SSM, intra-layer combination (https://arxiv.org/abs/2411.13676), intra-sequence combination appeared. The method is converting from attention to Mamba in the sequence.
</english>

#state-space-model 