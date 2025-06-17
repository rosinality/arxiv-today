https://arxiv.org/abs/2505.01618

*Don't be lazy: CompleteP enables compute-efficient deep transformers* (Nolan Dey, Bin Claire Zhang, Lorenzo Noci, Mufan Li, Blake Bordelon, Shane Bergsma, Cengiz Pehlevan, Boris Hanin, Joel Hestness)

> We study compute efficiency of LLM training when using different parameterizations, i.e., rules for adjusting model and optimizer hyperparameters (HPs) as model size changes. Some parameterizations fail to transfer optimal base HPs (such as learning rate) across changes in model depth, requiring practitioners to either re-tune these HPs as they scale up (expensive), or accept sub-optimal training when re-tuning is prohibitive. Even when they achieve HP transfer, we develop theory to show parameterizations may still exist in the lazy learning regime where layers learn only features close to their linearization, preventing effective use of depth and nonlinearity. Finally, we identify and adopt the unique parameterization we call CompleteP that achieves both depth-wise HP transfer and non-lazy learning in all layers. CompleteP enables a wider range of model width/depth ratios to remain compute-efficient, unlocking shapes better suited for different hardware settings and operational contexts. Moreover, CompleteP enables 12-34\% compute efficiency improvements over the prior state-of-the-art.

깊이 변화에 대해서도 적용 가능한 Hyperparameter Transfer. α = 1이 최적 세팅이라 결과적으로는 Residual Branch에 대한 Reweighting과 비슷하네요. 너비-깊이 비율을 조정할 수 있는 여지도 커진다고 합니다. 이것도 깊은 모델에 대한 안정화 테크닉과 비슷한 점이라고 생각할 수 있을 것 같군요.

<english>
Hyperparameter transformer that can be used depth variations. As α = 1 is optimal setting it is similar to reweighting for residual branches, in result. It also allows more space to adjust width-depth ratio. I think it can be also think as stabilization techniques for deep models.
</english>

#hyperparameter 