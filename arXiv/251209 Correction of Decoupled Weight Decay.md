https://arxiv.org/abs/2512.08217

*Correction of Decoupled Weight Decay* (Jason Chuan-Chih Chou)

> Decoupled weight decay, solely responsible for the performance advantage of AdamW over Adam, has long been set to proportional to learning rate $\gamma$ without questioning. Some researchers have recently challenged such assumption and argued that decoupled weight decay should be set $\propto \gamma^2$ instead based on orthogonality arguments at steady state. To the contrary, we find that eliminating the contribution of the perpendicular component of the update to the weight norm leads to little change to the training dynamics. Instead, we derive that decoupled weight decay $\propto \gamma^2$ results in stable weight norm based on the simple assumption that updates become independent of the weights at steady state, regardless of the nature of the optimizer. Based on the same assumption, we derive and empirically verify that the Total Update Contribution (TUC) of a minibatch under the Scion optimizer is better characterized by the momentum-dependent effective learning rate whose optimal value transfers and we show that decoupled weight decay $\propto \gamma^2$ leads to stable weight and gradient norms and allows us to better control the training dynamics and improve the model performance.

Extension on the necessity of weight decay scheduling proportional to the squared effective learning rate, for general optimizers.

#optimization 