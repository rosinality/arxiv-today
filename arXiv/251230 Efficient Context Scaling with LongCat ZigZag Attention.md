https://arxiv.org/abs/2512.23966

*Efficient Context Scaling with LongCat ZigZag Attention* (Chen Zhang, Yang Bai, Jiahuan Li, Anchun Gui, Keheng Wang, Feifan Liu, Guanyu Wu, Yuwei Jiang, Defei Bu, Li Wei, Haihang Jing, Hongyin Tang, Xin Chen, Xiangzhou Huang, Fengcun Li, Rongxiang Weng, Yulei Qian, Yifan Lu, Yerui Sun, Jingang Wang, Yuchen Xie, Xunliang Cai)

> We introduce LongCat ZigZag Attention (LoZA), which is a sparse attention scheme designed to transform any existing full-attention models into sparse versions with rather limited compute budget. In long-context scenarios, LoZA can achieve significant speed-ups both for prefill-intensive (e.g., retrieval-augmented generation) and decode-intensive (e.g., tool-integrated reasoning) cases. Specifically, by applying LoZA to LongCat-Flash during mid-training, we serve LongCat-Flash-Exp as a long-context foundation model that can swiftly process up to 1 million tokens, enabling efficient long-term reasoning and long-horizon agentic capabilities.

Sparse Attention 채택을 위한 미드트레이닝. Sink 블록과 Local Window 블록 여러 개를 결합한 고정된 Sparse Mask를 사용하는 것 같은데 다만 아주 명확하지는 않음.

Mid-training to adopt sparse attention. The sparse pattern seems like a fixed mask that mixes several local windows and a sink block, but the actual construction is a bit ambiguous.

#sparse-attention 