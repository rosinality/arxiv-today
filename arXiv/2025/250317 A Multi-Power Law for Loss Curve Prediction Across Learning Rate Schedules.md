https://arxiv.org/abs/2503.12811

*A Multi-Power Law for Loss Curve Prediction Across Learning Rate Schedules* (Kairong Luo, Haodong Wen, Shengding Hu, Zhenbo Sun, Zhiyuan Liu, Maosong Sun, Kaifeng Lyu, Wenguang Chen)

> Training large models is both resource-intensive and time-consuming, making it crucial to understand the quantitative relationship between model performance and hyperparameters. In this paper, we present an empirical law that describes how the pretraining loss of large language models evolves under different learning rate schedules, such as constant, cosine, and step decay schedules. Our proposed law takes a multi-power form, combining a power law based on the sum of learning rates and additional power laws to account for a loss reduction effect induced by learning rate decay. We extensively validate this law on various model sizes and architectures, and demonstrate that after fitting on a few learning rate schedules, the law accurately predicts the loss curves for unseen schedules of different shapes and horizons. Moreover, by minimizing the predicted final pretraining loss across learning rate schedules, we are able to find a schedule that outperforms the widely used cosine learning rate schedule. Interestingly, this automatically discovered schedule bears some resemblance to the recently proposed Warmup-Stable-Decay (WSD) schedule (Hu et al, 2024) but achieves a slightly lower final loss. We believe these results could offer valuable insights for understanding the dynamics of pretraining and designing learning rate schedules to improve efficiency.

LR Scheduling Scaling Law. 이전에 나왔던 Scaling Law보다 정확하다고 합니다. (https://arxiv.org/abs/2408.11029) 이를 기반으로 최적 스케줄을 추정했는데 WSD와 비슷한 형태군요.

<english>
Scaling law for LR schedules. The authors insist it is more accurate than scaling law came out previously (https://arxiv.org/abs/2408.11029). They optimized optimal schedule based on this, and it has similar form with WSD.
</english>

#scaling-law #hyperparameter 