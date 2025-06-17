https://arxiv.org/abs/2411.17470

*Towards Precise Scaling Laws for Video Diffusion Transformers* (Yuanyang Yin, Yaqi Zhao, Mingwu Zheng, Ke Lin, Jiarong Ou, Rui Chen, Victor Shea-Jay Huang, Jiahao Wang, Xin Tao, Pengfei Wan, Di Zhang, Baoqun Yin, Wentao Zhang, Kun Gai)

> Achieving optimal performance of video diffusion transformers within given data and compute budget is crucial due to their high training costs. This necessitates precisely determining the optimal model size and training hyperparameters before large-scale training. While scaling laws are employed in language models to predict performance, their existence and accurate derivation in visual generation models remain underexplored. In this paper, we systematically analyze scaling laws for video diffusion transformers and confirm their presence. Moreover, we discover that, unlike language models, video diffusion models are more sensitive to learning rate and batch size, two hyperparameters often not precisely modeled. To address this, we propose a new scaling law that predicts optimal hyperparameters for any model size and compute budget. Under these optimal settings, we achieve comparable performance and reduce inference costs by 40.1% compared to conventional scaling methods, within a compute budget of 1e10 TFlops. Furthermore, we establish a more generalized and precise relationship among validation loss, any model size, and compute budget. This enables performance prediction for non-optimal model sizes, which may also be appealed under practical inference cost constraints, achieving a better trade-off.

Video Diffusion에 대한 Scaling Law. 사실 가장 힘을 싣고 있는 것은 배치 크기와 Learning Rate에 대한 Scaling Law로 최적 하이퍼파라미터를 결정하는 부분이네요.

<english>
Scaling law for video diffusion. Actually the parts that authors most concentrated on is determining hyperparameters like batch sizes and learning rates using scaling law.
</english>

#diffusion #video-generation #scaling-law 