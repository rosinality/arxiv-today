https://arxiv.org/abs/2508.12880

*S^2-Guidance: Stochastic Self Guidance for Training-Free Enhancement of Diffusion Models* (Chubin Chen, Jiashu Zhu, Xiaokun Feng, Nisha Huang, Meiqi Wu, Fangyuan Mao, Jiahong Wu, Xiangxiang Chu, Xiu Li)

> Classifier-free Guidance (CFG) is a widely used technique in modern diffusion models for enhancing sample quality and prompt adherence. However, through an empirical analysis on Gaussian mixture modeling with a closed-form solution, we observe a discrepancy between the suboptimal results produced by CFG and the ground truth. The model's excessive reliance on these suboptimal predictions often leads to semantic incoherence and low-quality outputs. To address this issue, we first empirically demonstrate that the model's suboptimal predictions can be effectively refined using sub-networks of the model itself. Building on this insight, we propose S^2-Guidance, a novel method that leverages stochastic block-dropping during the forward process to construct stochastic sub-networks, effectively guiding the model away from potential low-quality predictions and toward high-quality outputs. Extensive qualitative and quantitative experiments on text-to-image and text-to-video generation tasks demonstrate that S^2-Guidance delivers superior performance, consistently surpassing CFG and other advanced guidance strategies. Our code will be released.

Stochastic Depth로 약한 모델을 만들어 가이드를 주는 방법.

Guiding sampling by using weak models constructed from stochastic depth.

#sampling #diffusion 